---
title: "Update workbookApplication"
description: "Update the properties of a workbookApplication object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookApplication

Namespace: microsoft.graph

Update the properties of a [workbookApplication](../resources/workbookapplication.md) object.

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
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/application
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookApplication](../resources/workbookapplication.md) object.

The following table shows the properties that are required when you create the [workbookApplication](../resources/workbookapplication.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|calculationMode|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookApplication](../resources/workbookapplication.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_workbookapplication"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/application
Content-type: application/json
Content-length: 109

{
  "@odata.type": "#microsoft.graph.workbookApplication",
  "calculationMode": "Calculation Mode value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 158

{
  "@odata.type": "#microsoft.graph.workbookApplication",
  "id": "bb8e86c0-86c0-bb8e-c086-8ebbc0868ebb",
  "calculationMode": "Calculation Mode value"
}
```

