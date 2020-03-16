---
title: "Get workbookWorksheet"
description: "Read properties and relationships of the workbookWorksheet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbookWorksheet

Namespace: microsoft.graph

Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.

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
GET /me/drive/items/{driveItemId}/workbook/worksheets/{workbookWorksheetId}
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/worksheet
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/worksheet
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/pivotTables/{workbookPivotTableId}/worksheet
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheet"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/worksheets/{workbookWorksheetId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookWorksheet",
    "id": "7026f5fd-f5fd-7026-fdf5-2670fdf52670",
    "name": "Name value",
    "position": 8,
    "visibility": "Visibility value"
  }
}
```

