---
title: "Get post"
description: "Read properties and relationships of the post object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get post

Namespace: microsoft.graph

Read properties and relationships of the [post](../resources/post.md) object.

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
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/inReplyTo
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
If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_post"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1087

{
  "value": {
    "@odata.type": "#microsoft.graph.post",
    "id": "93b58985-8985-93b5-8589-b5938589b593",
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "receivedDateTime": "2016-12-31T23:59:09.8646673+03:00",
    "hasAttachments": true,
    "from": {
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      }
    },
    "sender": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "conversationThreadId": "Conversation Thread Id value",
    "newParticipants": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "conversationId": "Conversation Id value"
  }
}
```

