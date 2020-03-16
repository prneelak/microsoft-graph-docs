---
title: "Update workbookChartLineFormat"
description: "Update the properties of a workbookChartLineFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartLineFormat

Namespace: microsoft.graph

Update the properties of a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/format/line
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/format/line
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/majorGridlines/format/line
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.

The following table shows the properties that are required when you create the [workbookChartLineFormat](../resources/workbookchartlineformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|color|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartLineFormat](../resources/workbookchartlineformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartlineformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/format/line
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.workbookChartLineFormat",
  "color": "Color value"
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
Content-Length: 141

{
  "@odata.type": "#microsoft.graph.workbookChartLineFormat",
  "id": "641ad4bf-d4bf-641a-bfd4-1a64bfd41a64",
  "color": "Color value"
}
```

