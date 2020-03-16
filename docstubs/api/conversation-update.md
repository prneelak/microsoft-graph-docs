---
title: "Update conversation"
description: "Update the properties of a conversation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update conversation

Namespace: microsoft.graph

Update the properties of a [conversation](../resources/conversation.md) object.

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
PATCH /groups/{groupsId}/conversations/{conversationId}
PATCH /me/joinedTeams/{groupId}/conversations/{conversationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [conversation](../resources/conversation.md) object.

The following table shows the properties that are required when you create the [conversation](../resources/conversation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|topic|String||
|hasAttachments|Boolean||
|lastDeliveredDateTime|DateTimeOffset||
|uniqueSenders|String collection||
|preview|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [conversation](../resources/conversation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_conversation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/groups/{groupsId}/conversations/{conversationId}
Content-type: application/json
Content-length: 260

{
  "@odata.type": "#microsoft.graph.conversation",
  "topic": "Topic value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2017-01-01T00:00:23.2016934+03:00",
  "uniqueSenders": [
    "Unique Senders value"
  ],
  "preview": "Preview value"
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
Content-Length: 309

{
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
```

