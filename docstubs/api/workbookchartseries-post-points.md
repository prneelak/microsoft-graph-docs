---
title: "Add points"
description: "Add points by posting to the points collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add points

Namespace: microsoft.graph

Add points by posting to the points collection.

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartPoint](../resources/workbookchartpoint.md) object.

The following table shows the properties that are required when you create the [workbookChartPoint](../resources/workbookchartpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|[Json](../resources/json.md)||



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartpoint_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points
Content-type: application/json
Content-length: 123

{
  "@odata.type": "#microsoft.graph.workbookChartPoint",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartpoint"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 172

{
  "@odata.type": "#microsoft.graph.workbookChartPoint",
  "id": "d2cc2820-2820-d2cc-2028-ccd22028ccd2",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

