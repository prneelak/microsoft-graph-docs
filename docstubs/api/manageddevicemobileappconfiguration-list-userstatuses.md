---
title: "List userStatuses"
description: "Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userStatuses

Namespace: microsoft.graph

Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.

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
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_manageddevicemobileappconfigurationuserstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddevicemobileappconfigurationuserstatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "8ecd4403-4403-8ecd-0344-cd8e0344cd8e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "String",
      "lastReportedDateTime": "2016-12-31T23:59:02.2314971+03:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```

