---
title: "Update workbookChartTitleFormat"
description: "Update the properties of a workbookChartTitleFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartTitleFormat

Namespace: microsoft.graph

Update the properties of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title/format
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.

The following table shows the properties that are required when you create the [workbookChartTitleFormat](../resources/workbookcharttitleformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookcharttitleformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title/format
Content-type: application/json
Content-length: 66

{
  "@odata.type": "#microsoft.graph.workbookChartTitleFormat"
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
  "@odata.type": "#microsoft.graph.workbookChartTitleFormat",
  "id": "d998f874-f874-d998-74f8-98d974f898d9"
}
```

