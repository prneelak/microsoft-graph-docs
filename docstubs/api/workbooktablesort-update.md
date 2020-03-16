---
title: "Update workbookTableSort"
description: "Update the properties of a workbookTableSort object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookTableSort

Namespace: microsoft.graph

Update the properties of a [workbookTableSort](../resources/workbooktablesort.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookTableSort](../resources/workbooktablesort.md) object.

The following table shows the properties that are required when you create the [workbookTableSort](../resources/workbooktablesort.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|fields|[workbookSortField](../resources/workbooksortfield.md) collection||
|matchCase|Boolean||
|method|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookTableSort](../resources/workbooktablesort.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbooktablesort"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
Content-type: application/json
Content-length: 485

{
  "@odata.type": "#microsoft.graph.workbookTableSort",
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
Content-Length: 534

{
  "@odata.type": "#microsoft.graph.workbookTableSort",
  "id": "c5cdf12d-f12d-c5cd-2df1-cdc52df1cdc5",
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
```

