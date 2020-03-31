---
title: "Update post"
description: "Update the properties of a post object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update post

Namespace: microsoft.graph

Update the properties of a [post](../resources/post.md) object.

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
PATCH /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
PATCH /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/inReplyTo
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [post](../resources/post.md) object.

The following table shows the properties that are required when you create the [post](../resources/post.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|body|[itemBody](../resources/itembody.md)||
|receivedDateTime|DateTimeOffset||
|hasAttachments|Boolean||
|from|[recipient](../resources/recipient.md)||
|sender|[recipient](../resources/recipient.md)||
|conversationThreadId|String||
|newParticipants|[recipient](../resources/recipient.md) collection||
|conversationId|String||
|importance|Enumeration| Possible values are: `low`, `normal`, `high`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [post](../resources/post.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_post"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
Content-type: application/json
Content-length: 857

{
  "@odata.type": "#microsoft.graph.post",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "receivedDateTime": "2017-01-01T00:03:20.0381972+03:00",
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
  "conversationId": "Conversation Id value",
  "importance": "String"
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
Content-Length: 1029

{
  "@odata.type": "#microsoft.graph.post",
  "id": "b286bea9-bea9-b286-a9be-86b2a9be86b2",
  "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "receivedDateTime": "2017-01-01T00:03:20.0381972+03:00",
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
  "conversationId": "Conversation Id value",
  "importance": "String"
}
```

