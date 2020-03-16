---
title: "Update workbookCommentReply"
description: "Update the properties of a workbookCommentReply object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookCommentReply

Namespace: microsoft.graph

Update the properties of a [workbookCommentReply](../resources/workbookcommentreply.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/comments/{workbookCommentId}/replies/{workbookCommentReplyId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookCommentReply](../resources/workbookcommentreply.md) object.

The following table shows the properties that are required when you create the [workbookCommentReply](../resources/workbookcommentreply.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|String||
|contentType|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookcommentreply"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/comments/{workbookCommentId}/replies/{workbookCommentReplyId}
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "content": "Content value",
  "contentType": "Content Type value"
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
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "id": "eacc1c2f-1c2f-eacc-2f1c-ccea2f1cccea",
  "content": "Content value",
  "contentType": "Content Type value"
}
```

