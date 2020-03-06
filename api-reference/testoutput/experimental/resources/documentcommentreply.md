---
title: "documentCommentReply resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# documentCommentReply resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get documentCommentReply](../api/documentcommentreply-get.md)|[documentCommentReply](../resources/documentcommentreply.md)|Read properties and relationships of the [documentCommentReply](../resources/documentcommentreply.md) object.|
|[Update documentCommentReply](../api/documentcommentreply-update.md)|[documentCommentReply](../resources/documentcommentreply.md)|Update the properties of a [documentCommentReply](../resources/documentcommentreply.md) object.|
|[List replies](../api/documentcomment-list-replies.md)|[documentCommentReply](../resources/documentcommentreply.md) collection|Get the documentCommentReplies from the replies navigation property.|
|[Add replies](../api/documentcomment-post-replies.md)|[documentCommentReply](../resources/documentcommentreply.md)|Add replies by posting to the replies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.documentCommentReply",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentCommentReply",
  "id": "String (identifier)",
  "content": "String"
}
```

