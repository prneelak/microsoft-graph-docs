---
title: "applyCellColorFilter"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# applyCellColorFilter

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter/applyCellColorFilter
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|color|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbookfilter_applycellcolorfilter"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter/applyCellColorFilter

Content-type: application/json
Content-length: 30

{
  "color": "Color value"
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
HTTP/1.1 204 No Content
```

