---
title: "List rows"
description: "Get the workbookTableRows from the rows navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List rows

Namespace: microsoft.graph

Get the workbookTableRows from the rows navigation property.

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
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows
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
If successful, this method returns a `200 OK` response code and a collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbooktablerow"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbooktablerow)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookTableRow",
      "id": "6a5a38c3-38c3-6a5a-c338-5a6ac3385a6a",
      "index": 5,
      "values": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```

