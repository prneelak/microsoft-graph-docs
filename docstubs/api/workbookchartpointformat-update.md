---
title: "Update workbookChartPointFormat"
description: "Update the properties of a workbookChartPointFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartPointFormat

Namespace: microsoft.graph

Update the properties of a [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points/{workbookChartPointId}/format
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.

The following table shows the properties that are required when you create the [workbookChartPointFormat](../resources/workbookchartpointformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartPointFormat](../resources/workbookchartpointformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartpointformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points/{workbookChartPointId}/format
Content-type: application/json
Content-length: 66

{
  "@odata.type": "#microsoft.graph.workbookChartPointFormat"
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
Content-Length: 115

{
  "@odata.type": "#microsoft.graph.workbookChartPointFormat",
  "id": "66005de1-5de1-6600-e15d-0066e15d0066"
}
```

