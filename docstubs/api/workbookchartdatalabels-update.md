---
title: "Update workbookChartDataLabels"
description: "Update the properties of a workbookChartDataLabels object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartDataLabels

Namespace: microsoft.graph

Update the properties of a [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/dataLabels
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.

The following table shows the properties that are required when you create the [workbookChartDataLabels](../resources/workbookchartdatalabels.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|position|String||
|separator|String||
|showBubbleSize|Boolean||
|showCategoryName|Boolean||
|showLegendKey|Boolean||
|showPercentage|Boolean||
|showSeriesName|Boolean||
|showValue|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartdatalabels"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/dataLabels
Content-type: application/json
Content-length: 291

{
  "@odata.type": "#microsoft.graph.workbookChartDataLabels",
  "position": "Position value",
  "separator": "Separator value",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
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
Content-Length: 340

{
  "@odata.type": "#microsoft.graph.workbookChartDataLabels",
  "id": "ec05a8e0-a8e0-ec05-e0a8-05ece0a805ec",
  "position": "Position value",
  "separator": "Separator value",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}
```

