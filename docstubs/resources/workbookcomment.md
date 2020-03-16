---
title: "workbookComment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookComment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookComment](../api/workbookcomment-get.md)|[workbookComment](../resources/workbookcomment.md)|Read properties and relationships of the [workbookComment](../resources/workbookcomment.md) object.|
|[Update workbookComment](../api/workbookcomment-update.md)|[workbookComment](../resources/workbookcomment.md)|Update the properties of a [workbookComment](../resources/workbookcomment.md) object.|
|[List replies](../api/workbookcomment-list-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md) collection|Get the workbookCommentReplies from the replies navigation property.|
|[Add replies](../api/workbookcomment-post-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Add replies by posting to the replies collection.|
|[List comments](../api/workbook-list-comments.md)|[workbookComment](../resources/workbookcomment.md) collection|Get the workbookComments from the comments navigation property.|
|[Add comments](../api/workbook-post-comments.md)|[workbookComment](../resources/workbookcomment.md)|Add comments by posting to the comments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|contentType|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|replies|[workbookCommentReply](../resources/workbookcommentreply.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookComment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookComment",
  "id": "String (identifier)",
  "content": "String",
  "contentType": "String"
}
```

