---
title: "Add conversations"
description: "Add conversations by posting to the conversations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add conversations

Namespace: microsoft.graph

Add conversations by posting to the conversations collection.

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
POST /groups/{groupsId}/conversations/$ref
POST /me/joinedTeams/{groupId}/conversations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [conversation](../resources/conversation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groups/{groupsId}/conversations
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
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
}
-->
``` http
HTTP/1.1 201 Created
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

