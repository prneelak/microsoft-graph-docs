---
title: "Add series"
description: "Add series by posting to the series collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add series

Namespace: microsoft.graph

Add series by posting to the series collection.

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartSeries](../resources/workbookchartseries.md) object.

The following table shows the properties that are required when you create the [workbookChartSeries](../resources/workbookchartseries.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartseries_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series
Content-type: application/json
Content-length: 86

{
  "@odata.type": "#microsoft.graph.workbookChartSeries",
  "name": "Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartseries"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 135

{
  "@odata.type": "#microsoft.graph.workbookChartSeries",
  "id": "c0d51c44-1c44-c0d5-441c-d5c0441cd5c0",
  "name": "Name value"
}
```

