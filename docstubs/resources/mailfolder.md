---
title: "mailFolder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mailFolder resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mailFolder](../api/mailfolder-get.md)|[mailFolder](../resources/mailfolder.md)|Read properties and relationships of the [mailFolder](../resources/mailfolder.md) object.|
|[Update mailFolder](../api/mailfolder-update.md)|[mailFolder](../resources/mailfolder.md)|Update the properties of a [mailFolder](../resources/mailfolder.md) object.|
|[delta](../api/mailfolder-delta.md)|[mailFolder](../resources/mailfolder.md) collection||
|[copy](../api/mailfolder-copy.md)|[mailFolder](../resources/mailfolder.md)||
|[move](../api/mailfolder-move.md)|[mailFolder](../resources/mailfolder.md)||
|[List singleValueExtendedProperties](../api/mailfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/mailfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/mailfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/mailfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List messages](../api/mailfolder-list-messages.md)|[message](../resources/message.md) collection|Get the messages from the messages navigation property.|
|[Add messages](../api/mailfolder-post-messages.md)|[message](../resources/message.md)|Add messages by posting to the messages collection.|
|[List messageRules](../api/mailfolder-list-messagerules.md)|[messageRule](../resources/messagerule.md) collection|Get the messageRules from the messageRules navigation property.|
|[Add messageRules](../api/mailfolder-post-messagerules.md)|[messageRule](../resources/messagerule.md)|Add messageRules by posting to the messageRules collection.|
|[List childFolders](../api/mailfolder-list-childfolders.md)|[mailFolder](../resources/mailfolder.md) collection|Get the mailFolders from the childFolders navigation property.|
|[Add childFolders](../api/mailfolder-post-childfolders.md)|[mailFolder](../resources/mailfolder.md)|Add childFolders by posting to the childFolders collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childFolderCount|Int32||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|parentFolderId|String||
|totalItemCount|Int32||
|unreadItemCount|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childFolders|[mailFolder](../resources/mailfolder.md) collection||
|messageRules|[messageRule](../resources/messagerule.md) collection||
|messages|[message](../resources/message.md) collection||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailFolder",
  "id": "String (identifier)",
  "displayName": "String",
  "parentFolderId": "String",
  "childFolderCount": 1024,
  "unreadItemCount": 1024,
  "totalItemCount": 1024
}
```

