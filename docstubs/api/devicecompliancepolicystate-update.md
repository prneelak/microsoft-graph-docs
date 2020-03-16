---
title: "Update deviceCompliancePolicyState"
description: "Update the properties of a deviceCompliancePolicyState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceCompliancePolicyState

Namespace: microsoft.graph

Update the properties of a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.

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
PATCH /me/managedDevices/{managedDeviceId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settingStates|[deviceCompliancePolicySettingState](../resources/devicecompliancepolicysettingstate.md) collection||
|displayName|String|The name of the policy for this policyBase|
|version|Int32|The version of the policy|
|platformType|Enumeration|Platform type that the policy applies to. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|state|Enumeration|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32|Count of how many setting a policy holds|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicecompliancepolicystate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
Content-type: application/json
Content-length: 962

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1011

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
```

