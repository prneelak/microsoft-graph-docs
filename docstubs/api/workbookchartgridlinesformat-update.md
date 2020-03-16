---
title: "Update workbookChartGridlinesFormat"
description: "Update the properties of a workbookChartGridlinesFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartGridlinesFormat

Namespace: microsoft.graph

Update the properties of a [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/majorGridlines/format
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.

The following table shows the properties that are required when you create the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartgridlinesformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/majorGridlines/format
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.workbookChartGridlinesFormat"
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
Content-Length: 119

{
  "@odata.type": "#microsoft.graph.workbookChartGridlinesFormat",
  "id": "fd3403f9-03f9-fd34-f903-34fdf90334fd"
}
```

