---
title: "List deviceCompliancePolicyStates"
description: "Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceCompliancePolicyStates

Namespace: microsoft.graph

Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/managedDevices/{managedDeviceId}/deviceCompliancePolicyStates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicecompliancepolicystate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/deviceCompliancePolicyStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicecompliancepolicystate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1164

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
      "id": "cf104914-4914-cf10-1449-10cf144910cf",
      "settingStates": [
        {
          "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
          "setting": "Setting value",
          "settingName": "Setting Name value",
          "instanceDisplayName": "Instance Display Name value",
          "state": "String",
          "errorCode": 9,
          "errorDescription": "Error Description value",
          "userId": "User Id value",
          "userName": "User Name value",
          "userEmail": "User Email value",
          "userPrincipalName": "User Principal Name value",
          "sources": [
            {
              "@odata.type": "microsoft.graph.settingSource",
              "id": "Id value",
              "displayName": "Display Name value"
            }
          ],
          "currentValue": "Current Value value"
        }
      ],
      "displayName": "Display Name value",
      "version": 7,
      "platformType": "String",
      "state": "String",
      "settingCount": 12
    }
  ]
}
```

