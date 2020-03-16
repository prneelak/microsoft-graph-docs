---
title: "Add names"
description: "Add names by posting to the names collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add names

Namespace: microsoft.graph

Add names by posting to the names collection.

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/names/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookNamedItem](../resources/workbooknameditem.md) object.

The following table shows the properties that are required when you create the [workbookNamedItem](../resources/workbooknameditem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|comment|String||
|name|String||
|scope|String||
|type|String||
|value|[Json](../resources/json.md)||
|visible|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbooknameditem_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/names
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "comment": "Comment value",
  "name": "Name value",
  "scope": "Scope value",
  "type": "Type value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": true
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
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
```

