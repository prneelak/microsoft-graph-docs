---
title: "post resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# post resource type


Namespace: microsoft.graph




Inherits from [outlookItem](../resources/outlookitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get post](../api/post-get.md)|[post](../resources/post.md)|Read properties and relationships of the [post](../resources/post.md) object.|
|[Update post](../api/post-update.md)|[post](../resources/post.md)|Update the properties of a [post](../resources/post.md) object.|
|[reply](../api/post-reply.md)|None||
|[forward](../api/post-forward.md)|None||
|[Get post](../api/post-get.md)|[post](../resources/post.md)|Read properties and relationships of the [post](../resources/post.md) object.|
|[List singleValueExtendedProperties](../api/post-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/post-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/post-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/post-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List extensions](../api/post-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/post-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List attachments](../api/post-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/post-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|
|[List posts](../api/conversationthread-list-posts.md)|[post](../resources/post.md) collection|Get the posts from the posts navigation property.|
|[Add posts](../api/conversationthread-post-posts.md)|[post](../resources/post.md)|Add posts by posting to the posts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)||
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|conversationId|String||
|conversationThreadId|String||
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|from|[recipient](../resources/recipient.md)||
|hasAttachments|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|newParticipants|[recipient](../resources/recipient.md) collection||
|receivedDateTime|DateTimeOffset||
|sender|[recipient](../resources/recipient.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection||
|extensions|[extension](../resources/extension.md) collection||
|inReplyTo|[post](../resources/post.md)||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.post",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.post",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ],
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "String"
  },
  "receivedDateTime": "String (timestamp)",
  "hasAttachments": true,
  "from": {
    "@odata.type": "microsoft.graph.recipient",
    "emailAddress": {
      "@odata.type": "microsoft.graph.emailAddress",
      "address": "String"
    }
  },
  "sender": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "conversationThreadId": "String",
  "newParticipants": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "conversationId": "String"
}
```

