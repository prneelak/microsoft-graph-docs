---
title: "conversationThread resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conversationThread resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get conversationThread](../api/conversationthread-get.md)|[conversationThread](../resources/conversationthread.md)|Read properties and relationships of the [conversationThread](../resources/conversationthread.md) object.|
|[Update conversationThread](../api/conversationthread-update.md)|[conversationThread](../resources/conversationthread.md)|Update the properties of a [conversationThread](../resources/conversationthread.md) object.|
|[reply](../api/conversationthread-reply.md)|None||
|[List posts](../api/conversationthread-list-posts.md)|[post](../resources/post.md) collection|Get the posts from the posts navigation property.|
|[Add posts](../api/conversationthread-post-posts.md)|[post](../resources/post.md)|Add posts by posting to the posts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|ccRecipients|[recipient](../resources/recipient.md) collection||
|hasAttachments|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|isLocked|Boolean||
|lastDeliveredDateTime|DateTimeOffset||
|preview|String||
|topic|String||
|toRecipients|[recipient](../resources/recipient.md) collection||
|uniqueSenders|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|posts|[post](../resources/post.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationThread",
  "id": "String (identifier)",
  "toRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "topic": "String",
  "hasAttachments": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "uniqueSenders": [
    "String"
  ],
  "ccRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "preview": "String",
  "isLocked": true
}
```

