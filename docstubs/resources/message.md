---
title: "message resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# message resource type


Namespace: microsoft.graph




Inherits from [outlookItem](../resources/outlookitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get message](../api/message-get.md)|[message](../resources/message.md)|Read properties and relationships of the [message](../resources/message.md) object.|
|[Update message](../api/message-update.md)|[message](../resources/message.md)|Update the properties of a [message](../resources/message.md) object.|
|[createReply](../api/message-createreply.md)|[message](../resources/message.md)||
|[createReplyAll](../api/message-createreplyall.md)|[message](../resources/message.md)||
|[createForward](../api/message-createforward.md)|[message](../resources/message.md)||
|[send](../api/message-send.md)|None||
|[copy](../api/message-copy.md)|[message](../resources/message.md)||
|[move](../api/message-move.md)|[message](../resources/message.md)||
|[reply](../api/message-reply.md)|None||
|[replyAll](../api/message-replyall.md)|None||
|[forward](../api/message-forward.md)|None||
|[delta](../api/message-delta.md)|[message](../resources/message.md) collection||
|[List singleValueExtendedProperties](../api/message-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/message-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/message-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/message-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List attachments](../api/message-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/message-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|
|[List extensions](../api/message-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/message-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bccRecipients|[recipient](../resources/recipient.md) collection||
|body|[itemBody](../resources/itembody.md)||
|bodyPreview|String||
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection||
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|conversationId|String||
|conversationIndex|Binary||
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|flag|[followupFlag](../resources/followupflag.md)||
|from|[recipient](../resources/recipient.md)||
|hasAttachments|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration|. Possible values are: `low`, `normal`, `high`.|
|inferenceClassification|Enumeration|. Possible values are: `focused`, `other`.|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection||
|internetMessageId|String||
|isDeliveryReceiptRequested|Boolean||
|isDraft|Boolean||
|isRead|Boolean||
|isReadReceiptRequested|Boolean||
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|parentFolderId|String||
|receivedDateTime|DateTimeOffset||
|replyTo|[recipient](../resources/recipient.md) collection||
|sender|[recipient](../resources/recipient.md)||
|sentDateTime|DateTimeOffset||
|subject|String||
|toRecipients|[recipient](../resources/recipient.md) collection||
|uniqueBody|[itemBody](../resources/itembody.md)||
|webLink|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection||
|extensions|[extension](../resources/extension.md) collection||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.message",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ],
  "receivedDateTime": "String (timestamp)",
  "sentDateTime": "String (timestamp)",
  "hasAttachments": true,
  "internetMessageId": "String",
  "internetMessageHeaders": [
    {
      "@odata.type": "microsoft.graph.internetMessageHeader",
      "name": "String",
      "value": "String"
    }
  ],
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "String"
  },
  "bodyPreview": "String",
  "importance": "String",
  "parentFolderId": "String",
  "sender": {
    "@odata.type": "microsoft.graph.recipient",
    "emailAddress": {
      "@odata.type": "microsoft.graph.emailAddress",
      "address": "String"
    }
  },
  "from": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "toRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "ccRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "bccRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "replyTo": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "conversationId": "String",
  "conversationIndex": "binary",
  "uniqueBody": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "isDeliveryReceiptRequested": true,
  "isReadReceiptRequested": true,
  "isRead": true,
  "isDraft": true,
  "webLink": "String",
  "inferenceClassification": "String",
  "flag": {
    "@odata.type": "microsoft.graph.followupFlag",
    "completedDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "dueDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "startDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "flagStatus": "String"
  }
}
```

