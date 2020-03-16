---
title: "attachment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# attachment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get attachment](../api/attachment-get.md)|[attachment](../resources/attachment.md)|Read properties and relationships of the [attachment](../resources/attachment.md) object.|
|[List attachments](../api/event-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/event-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentType|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isInline|Boolean||
|lastModifiedDateTime|DateTimeOffset||
|name|String||
|size|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "contentType": "String",
  "size": 1024,
  "isInline": true
}
```

