---
title: "Create workbookNamedItem"
description: "Create a new workbookNamedItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookNamedItem

Namespace: microsoft.graph

Create a new [workbookNamedItem](../resources/workbooknameditem.md) object.

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
POST /me/drive/items/{driveItemId}/workbook/names
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/names
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names
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
  "id": "815ef7e7-f7e7-815e-e7f7-5e81e7f75e81",
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

