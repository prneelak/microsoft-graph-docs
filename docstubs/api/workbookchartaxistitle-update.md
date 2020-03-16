---
title: "Update workbookChartAxisTitle"
description: "Update the properties of a workbookChartAxisTitle object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartAxisTitle

Namespace: microsoft.graph

Update the properties of a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/title
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.

The following table shows the properties that are required when you create the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|text|String||
|visible|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartaxistitle"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/title
Content-type: application/json
Content-length: 109

{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitle",
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
Content-Length: 158

{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitle",
  "id": "d87229ba-29ba-d872-ba29-72d8ba2972d8",
  "text": "Text value",
  "visible": true
}
```

