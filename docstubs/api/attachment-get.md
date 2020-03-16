---
title: "Get attachment"
description: "Read properties and relationships of the attachment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get attachment

Namespace: microsoft.graph

Read properties and relationships of the [attachment](../resources/attachment.md) object.

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
GET /me/messages/{messageId}/attachments/{attachmentId}
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/attachments/{attachmentId}
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/attachments/{attachmentId}
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
If successful, this method returns a `200 OK` response code and [attachment](../resources/attachment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_attachment"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/messages/{messageId}/attachments/{attachmentId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": {
    "@odata.type": "#microsoft.graph.attachment",
    "id": "5a5bd3be-d3be-5a5b-bed3-5b5abed35b5a",
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
    "name": "Name value",
    "contentType": "Content Type value",
    "size": 4,
    "isInline": true
  }
}
```

