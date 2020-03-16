---
title: "add"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# add

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
POST /me/drive/items/{driveItemId}/workbook/names/add
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/names/add
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|name|String||
|reference|[Json](../resources/json.md)||
|comment|String||



## Response
If successful, this action returns a `200 OK` response code and a [workbookNamedItem](../resources/workbooknameditem.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbooknameditem_add"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/add

Content-type: application/json
Content-length: 126

{
  "name": "Name value",
  "reference": {
    "@odata.type": "microsoft.graph.Json"
  },
  "comment": "Comment value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooknameditem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 338

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "id": "f13b38bd-38bd-f13b-bd38-3bf1bd383bf1",
    "comment": "Comment value",
    "name": "Name value",
    "scope": "Scope value",
    "type": "Type value",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    },
    "visible": true
  }
}
```

