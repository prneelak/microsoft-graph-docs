---
title: "Get workbookCommentReply"
description: "Read properties and relationships of the workbookCommentReply object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbookCommentReply

Namespace: microsoft.graph

Read properties and relationships of the [workbookCommentReply](../resources/workbookcommentreply.md) object.

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
GET /me/drive/items/{driveItemId}/workbook/comments/{workbookCommentId}/replies/{workbookCommentReplyId}
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
If successful, this method returns a `200 OK` response code and [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/comments/{workbookCommentId}/replies/{workbookCommentReplyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookCommentReply",
    "id": "eacc1c2f-1c2f-eacc-2f1c-ccea2f1cccea",
    "content": "Content value",
    "contentType": "Content Type value"
  }
}
```

