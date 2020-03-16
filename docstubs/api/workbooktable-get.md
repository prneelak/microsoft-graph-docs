---
title: "Get workbookTable"
description: "Read properties and relationships of the workbookTable object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbookTable

Namespace: microsoft.graph

Read properties and relationships of the [workbookTable](../resources/workbooktable.md) object.

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
GET /me/drive/items/{driveItemId}/workbook/tables/{workbookTableId}
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}
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
If successful, this method returns a `200 OK` response code and [workbookTable](../resources/workbooktable.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbooktable"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/tables/{workbookTableId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 431

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookTable",
    "id": "da455bba-5bba-da45-ba5b-45daba5b45da",
    "highlightFirstColumn": true,
    "highlightLastColumn": true,
    "legacyId": "Legacy Id value",
    "name": "Name value",
    "showBandedColumns": true,
    "showBandedRows": true,
    "showFilterButton": true,
    "showHeaders": true,
    "showTotals": true,
    "style": "Style value"
  }
}
```

