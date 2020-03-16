---
title: "Add charts"
description: "Add charts by posting to the charts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add charts

Namespace: microsoft.graph

Add charts by posting to the charts collection.

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChart](../resources/workbookchart.md) object.

The following table shows the properties that are required when you create the [workbookChart](../resources/workbookchart.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|height|Double||
|left|Double||
|name|String||
|top|Double||
|width|Double||



## Response
If successful, this method returns a `201 Created` response code and a [workbookChart](../resources/workbookchart.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchart_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.workbookChart",
  "height": "Double",
  "left": "Double",
  "name": "Name value",
  "top": "Double",
  "width": "Double"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchart"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.workbookChart",
  "id": "3debb33b-b33b-3deb-3bb3-eb3d3bb3eb3d",
  "height": "Double",
  "left": "Double",
  "name": "Name value",
  "top": "Double",
  "width": "Double"
}
```

