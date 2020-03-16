---
title: "Update workbookChartAxisTitleFormat"
description: "Update the properties of a workbookChartAxisTitleFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartAxisTitleFormat

Namespace: microsoft.graph

Update the properties of a [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/title/format
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.

The following table shows the properties that are required when you create the [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartaxistitleformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/title/format
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitleFormat"
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
  "@odata.type": "#microsoft.graph.workbookChartAxisTitleFormat",
  "id": "c62a9351-9351-c62a-5193-2ac651932ac6"
}
```

