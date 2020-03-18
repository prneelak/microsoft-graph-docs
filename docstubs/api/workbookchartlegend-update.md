---
title: "Update workbookChartLegend"
description: "Update the properties of a workbookChartLegend object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartLegend

Namespace: microsoft.graph

Update the properties of a [workbookChartLegend](../resources/workbookchartlegend.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/legend
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartLegend](../resources/workbookchartlegend.md) object.

The following table shows the properties that are required when you create the [workbookChartLegend](../resources/workbookchartlegend.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|overlay|Boolean||
|position|String||
|visible|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartlegend"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/legend
Content-type: application/json
Content-length: 134

{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "overlay": true,
  "position": "Position value",
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
Content-Length: 183

{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "id": "c9ef7c47-7c47-c9ef-477c-efc9477cefc9",
  "overlay": true,
  "position": "Position value",
  "visible": true
}
```

