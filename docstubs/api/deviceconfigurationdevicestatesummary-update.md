---
title: "Update deviceConfigurationDeviceStateSummary"
description: "Update the properties of a deviceConfigurationDeviceStateSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceConfigurationDeviceStateSummary

Namespace: microsoft.graph

Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.

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
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|unknownDeviceCount|Int32|Number of unknown devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|compliantDeviceCount|Int32|Number of compliant devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|errorDeviceCount|Int32|Number of error devices|
|conflictDeviceCount|Int32|Number of conflict devices|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deviceconfigurationdevicestatesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
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
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "842c50cb-50cb-842c-cb50-2c84cb502c84",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

