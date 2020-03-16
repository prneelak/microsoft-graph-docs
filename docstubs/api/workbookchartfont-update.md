---
title: "Update workbookChartFont"
description: "Update the properties of a workbookChartFont object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartFont

Namespace: microsoft.graph

Update the properties of a [workbookChartFont](../resources/workbookchartfont.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/format/font
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title/format/font
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/legend/format/font
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/dataLabels/format/font
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/format/font
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/title/format/font
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartFont](../resources/workbookchartfont.md) object.

The following table shows the properties that are required when you create the [workbookChartFont](../resources/workbookchartfont.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|bold|Boolean||
|color|String||
|italic|Boolean||
|name|String||
|size|Double||
|underline|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartFont](../resources/workbookchartfont.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartfont"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/format/font
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.workbookChartFont",
  "bold": true,
  "color": "Color value",
  "italic": true,
  "name": "Name value",
  "size": "Double",
  "underline": "Underline value"
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
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.workbookChartFont",
  "id": "4ee843dd-43dd-4ee8-dd43-e84edd43e84e",
  "bold": true,
  "color": "Color value",
  "italic": true,
  "name": "Name value",
  "size": "Double",
  "underline": "Underline value"
}
```

