---
title: "Create messages"
description: "Create a new messages object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create messages

Namespace: microsoft.graph

Create a new messages object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/channels/{channelId}/messages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [chatMessage](../resources/chatmessage.md) object.

The following table shows the properties that are required when you create the [chatMessage](../resources/chatmessage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|replyToId|String|**TODO: Add Description**|
|from|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|etag|String|**TODO: Add Description**|
|messageType|chatMessageType|**TODO: Add Description**. Possible values are: `message`, `chatEvent`, `typing`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|summary|String|**TODO: Add Description**|
|attachments|[chatMessageAttachment](../resources/chatmessageattachment.md) collection|**TODO: Add Description**|
|mentions|[chatMessageMention](../resources/chatmessagemention.md) collection|**TODO: Add Description**|
|importance|chatMessageImportance|**TODO: Add Description**. Possible values are: `normal`, `high`, `urgent`, `unknownFutureValue`.|
|policyViolation|[chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md)|**TODO: Add Description**|
|reactions|[chatMessageReaction](../resources/chatmessagereaction.md) collection|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [chatMessage](../resources/chatmessage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamsId}/channels/{channelId}/messages
Content-Type: application/json
Content-length: 819

{
  "@odata.type": "#microsoft.graph.chatMessage",
  "replyToId": "String",
  "from": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "etag": "String",
  "messageType": "String",
  "deletedDateTime": "String (timestamp)",
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "summary": "String",
  "attachments": [
    {
      "@odata.type": "microsoft.graph.chatMessageAttachment"
    }
  ],
  "mentions": [
    {
      "@odata.type": "microsoft.graph.chatMessageMention"
    }
  ],
  "importance": "String",
  "policyViolation": {
    "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
  },
  "reactions": [
    {
      "@odata.type": "microsoft.graph.chatMessageReaction"
    }
  ],
  "locale": "String",
  "webUrl": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatmessage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.chatMessage",
  "id": "8597c951-c951-8597-51c9-978551c99785",
  "replyToId": "String",
  "from": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "etag": "String",
  "messageType": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "summary": "String",
  "attachments": [
    {
      "@odata.type": "microsoft.graph.chatMessageAttachment"
    }
  ],
  "mentions": [
    {
      "@odata.type": "microsoft.graph.chatMessageMention"
    }
  ],
  "importance": "String",
  "policyViolation": {
    "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
  },
  "reactions": [
    {
      "@odata.type": "microsoft.graph.chatMessageReaction"
    }
  ],
  "locale": "String",
  "webUrl": "String"
}
```

