---
title: "List workbookTableSorts"
description: "List properties and relationships of the workbookTableSort objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookTableSorts

Namespace: microsoft.graph

List properties and relationships of the [workbookTableSort](../resources/workbooktablesort.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookTableSort not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookTableSort](../resources/workbooktablesort.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbooktablesort"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookTableSort not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbooktablesort)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 643

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookTableSort",
      "id": "d7d09e99-9e99-d7d0-999e-d0d7999ed0d7",
      "fields": [
        {
          "@odata.type": "microsoft.graph.workbookSortField",
          "ascending": true,
          "color": "Color value",
          "dataOption": "Data Option value",
          "icon": {
            "@odata.type": "microsoft.graph.workbookIcon",
            "index": 5,
            "set": "Set value"
          },
          "key": 3,
          "sortOn": "Sort On value"
        }
      ],
      "matchCase": true,
      "method": "Method value"
    }
  ]
}
```

