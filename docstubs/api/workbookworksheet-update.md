---
title: "Update workbookWorksheet"
description: "Update the properties of a workbookWorksheet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookWorksheet

Namespace: microsoft.graph

Update the properties of a [workbookWorksheet](../resources/workbookworksheet.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/worksheets/{workbookWorksheetId}
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/worksheet
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/worksheet
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/pivotTables/{workbookPivotTableId}/worksheet
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookWorksheet](../resources/workbookworksheet.md) object.

The following table shows the properties that are required when you create the [workbookWorksheet](../resources/workbookworksheet.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|position|Int32||
|visibility|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookworksheet"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/worksheets/{workbookWorksheetId}
Content-type: application/json
Content-length: 139

{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "name": "Name value",
  "position": 8,
  "visibility": "Visibility value"
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
Content-Length: 188

{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "id": "7026f5fd-f5fd-7026-fdf5-2670fdf52670",
  "name": "Name value",
  "position": 8,
  "visibility": "Visibility value"
}
```

