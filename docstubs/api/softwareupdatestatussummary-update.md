---
title: "Update softwareUpdateStatusSummary"
description: "Update the properties of a softwareUpdateStatusSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update softwareUpdateStatusSummary

Namespace: microsoft.graph

Update the properties of a [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.

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
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.

The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The name of the policy.|
|compliantDeviceCount|Int32|Number of compliant devices.|
|nonCompliantDeviceCount|Int32|Number of non compliant devices.|
|remediatedDeviceCount|Int32|Number of remediated devices.|
|errorDeviceCount|Int32|Number of devices had error.|
|unknownDeviceCount|Int32|Number of unknown devices.|
|conflictDeviceCount|Int32|Number of conflict devices.|
|notApplicableDeviceCount|Int32|Number of not applicable devices.|
|compliantUserCount|Int32|Number of compliant users.|
|nonCompliantUserCount|Int32|Number of non compliant users.|
|remediatedUserCount|Int32|Number of remediated users.|
|errorUserCount|Int32|Number of users had error.|
|unknownUserCount|Int32|Number of unknown users.|
|conflictUserCount|Int32|Number of conflict users.|
|notApplicableUserCount|Int32|Number of not applicable users.|



## Response
If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_softwareupdatestatussummary"
}
-->
``` http

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
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "a1f706e8-06e8-a1f7-e806-f7a1e806f7a1",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

