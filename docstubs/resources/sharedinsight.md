---
title: "sharedInsight resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharedInsight resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sharedInsight](../api/sharedinsight-get.md)|[sharedInsight](../resources/sharedinsight.md)|Read properties and relationships of the [sharedInsight](../resources/sharedinsight.md) object.|
|[Update sharedInsight](../api/sharedinsight-update.md)|[sharedInsight](../resources/sharedinsight.md)|Update the properties of a [sharedInsight](../resources/sharedinsight.md) object.|
|[Get entity](../api/entity-get.md)|[entity](../resources/entity.md)|Read properties and relationships of the [entity](../resources/entity.md) object.|
|[Get entity](../api/entity-get.md)|[entity](../resources/entity.md)|Read properties and relationships of the [entity](../resources/entity.md) object.|
|[List shared](../api/officegraphinsights-list-shared.md)|[sharedInsight](../resources/sharedinsight.md) collection|Get the sharedInsights from the shared navigation property.|
|[Add shared](../api/officegraphinsights-post-shared.md)|[sharedInsight](../resources/sharedinsight.md)|Add shared by posting to the shared collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastShared|[sharingDetail](../resources/sharingdetail.md)||
|resourceReference|[resourceReference](../resources/resourcereference.md)||
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)||
|sharingHistory|[sharingDetail](../resources/sharingdetail.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|lastSharedMethod|[entity](../resources/entity.md)||
|resource|[entity](../resources/entity.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "id": "String (identifier)",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail",
    "sharedBy": {
      "@odata.type": "microsoft.graph.insightIdentity",
      "displayName": "String",
      "id": "String",
      "address": "String"
    },
    "sharedDateTime": "String (timestamp)",
    "sharingSubject": "String",
    "sharingType": "String",
    "sharingReference": {
      "@odata.type": "microsoft.graph.resourceReference",
      "webUrl": "String",
      "type": "String"
    }
  },
  "sharingHistory": [
    {
      "@odata.type": "microsoft.graph.sharingDetail"
    }
  ],
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization",
    "title": "String",
    "mediaType": "String",
    "previewImageUrl": "String",
    "previewText": "String",
    "containerWebUrl": "String",
    "containerDisplayName": "String",
    "containerType": "String"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference"
  }
}
```

