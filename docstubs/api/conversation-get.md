---
title: "Get conversation"
description: "Read properties and relationships of the conversation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get conversation

Namespace: microsoft.graph

Read properties and relationships of the [conversation](../resources/conversation.md) object.

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
GET /groups/{groupsId}/conversations/{conversationId}
GET /me/joinedTeams/{groupId}/conversations/{conversationId}
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
If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/conversations/{conversationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.conversation",
    "id": "cb23a026-a026-cb23-26a0-23cb26a023cb",
    "topic": "Topic value",
    "hasAttachments": true,
    "lastDeliveredDateTime": "2017-01-01T00:00:23.2016934+03:00",
    "uniqueSenders": [
      "Unique Senders value"
    ],
    "preview": "Preview value"
  }
}
```

