---
title: "Update deviceConfigurationDeviceOverview"
description: "Update the properties of a deviceConfigurationDeviceOverview object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceConfigurationDeviceOverview

Namespace: microsoft.graph

Update the properties of a [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|pendingCount|Int32|Number of pending devices|
|notApplicableCount|Int32|Number of not applicable devices|
|successCount|Int32|Number of succeeded devices|
|errorCount|Int32|Number of error devices|
|failedCount|Int32|Number of failed devices|
|lastUpdateDateTime|DateTimeOffset|Last update time|
|configurationVersion|Int32|Version of the policy for that overview|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deviceconfigurationdeviceoverview"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:59:58.1382181+03:00",
  "configurationVersion": 4
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
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "61769ded-9ded-6176-ed9d-7661ed9d7661",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:59:58.1382181+03:00",
  "configurationVersion": 4
}
```

