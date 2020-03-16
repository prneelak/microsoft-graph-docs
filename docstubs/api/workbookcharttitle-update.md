---
title: "Update workbookChartTitle"
description: "Update the properties of a workbookChartTitle object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartTitle

Namespace: microsoft.graph

Update the properties of a [workbookChartTitle](../resources/workbookcharttitle.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartTitle](../resources/workbookcharttitle.md) object.

The following table shows the properties that are required when you create the [workbookChartTitle](../resources/workbookcharttitle.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|overlay|Boolean||
|text|String||
|visible|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookcharttitle"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "overlay": true,
  "text": "Text value",
  "visible": true
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
Content-Length: 174

{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "id": "d6f37d47-7d47-d6f3-477d-f3d6477df3d6",
  "overlay": true,
  "text": "Text value",
  "visible": true
}
```

