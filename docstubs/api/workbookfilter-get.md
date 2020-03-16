---
title: "Get workbookFilter"
description: "Read properties and relationships of the workbookFilter object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbookFilter

Namespace: microsoft.graph

Read properties and relationships of the [workbookFilter](../resources/workbookfilter.md) object.

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
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
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
If successful, this method returns a `200 OK` response code and [workbookFilter](../resources/workbookfilter.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookfilter"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFilter"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookFilter",
    "id": "ecbe6d20-6d20-ecbe-206d-beec206dbeec",
    "criteria": {
      "@odata.type": "microsoft.graph.workbookFilterCriteria",
      "color": "Color value",
      "criterion1": "Criterion1 value",
      "criterion2": "Criterion2 value",
      "dynamicCriteria": "Dynamic Criteria value",
      "filterOn": "Filter On value",
      "icon": {
        "@odata.type": "microsoft.graph.workbookIcon",
        "index": 5,
        "set": "Set value"
      },
      "operator": "Operator value",
      "values": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  }
}
```

