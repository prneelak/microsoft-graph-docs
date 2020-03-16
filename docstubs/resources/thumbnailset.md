---
title: "thumbnailSet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# thumbnailSet resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get thumbnailSet](../api/thumbnailset-get.md)|[thumbnailSet](../resources/thumbnailset.md)|Read properties and relationships of the [thumbnailSet](../resources/thumbnailset.md) object.|
|[Update thumbnailSet](../api/thumbnailset-update.md)|[thumbnailSet](../resources/thumbnailset.md)|Update the properties of a [thumbnailSet](../resources/thumbnailset.md) object.|
|[List thumbnails](../api/driveitem-list-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md) collection|Get the thumbnailSets from the thumbnails navigation property.|
|[Add thumbnails](../api/driveitem-post-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md)|Add thumbnails by posting to the thumbnails collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|large|[thumbnail](../resources/thumbnail.md)||
|medium|[thumbnail](../resources/thumbnail.md)||
|small|[thumbnail](../resources/thumbnail.md)||
|source|[thumbnail](../resources/thumbnail.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.thumbnailSet",
  "id": "String (identifier)",
  "large": {
    "@odata.type": "microsoft.graph.thumbnail"
  },
  "medium": {
    "@odata.type": "microsoft.graph.thumbnail"
  },
  "small": {
    "@odata.type": "microsoft.graph.thumbnail"
  },
  "source": {
    "@odata.type": "microsoft.graph.thumbnail"
  }
}
```

