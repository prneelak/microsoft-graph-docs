---
title: "range"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# range

Namespace: microsoft.graph



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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/range
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [workbookRange](../resources/workbookrange.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbooktablecolumn_range"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/range
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrange"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 898

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookRange",
    "id": "18cf561c-561c-18cf-1c56-cf181c56cf18",
    "address": "Address value",
    "addressLocal": "Address Local value",
    "cellCount": 9,
    "columnCount": 11,
    "columnHidden": true,
    "columnIndex": 11,
    "formulas": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasLocal": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasR1C1": {
      "@odata.type": "microsoft.graph.Json"
    },
    "hidden": true,
    "numberFormat": {
      "@odata.type": "microsoft.graph.Json"
    },
    "rowCount": 8,
    "rowHidden": true,
    "rowIndex": 8,
    "text": {
      "@odata.type": "microsoft.graph.Json"
    },
    "valueTypes": {
      "@odata.type": "microsoft.graph.Json"
    },
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

