---
title: "Add deviceStatuses"
description: "Add deviceStatuses by posting to the deviceStatuses collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceStatuses

Namespace: microsoft.graph

Add deviceStatuses by posting to the deviceStatuses collection.

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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceDisplayName|String|Device name of the DevicePolicyStatus.|
|userName|String|The User Name that is being reported|
|deviceModel|String|The device model that is being reported|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|userPrincipalName|String|UserPrincipalName.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceconfigurationdevicestatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 423

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2017-01-01T00:03:23.4975081+03:00",
  "status": "String",
  "lastReportedDateTime": "2016-12-31T23:57:17.1308941+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceconfigurationdevicestatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 472

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "565562b6-62b6-5655-b662-5556b6625556",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2017-01-01T00:03:23.4975081+03:00",
  "status": "String",
  "lastReportedDateTime": "2016-12-31T23:57:17.1308941+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

