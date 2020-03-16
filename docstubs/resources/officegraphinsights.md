---
title: "officeGraphInsights resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# officeGraphInsights resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get officeGraphInsights](../api/officegraphinsights-get.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Read properties and relationships of the [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[Update officeGraphInsights](../api/officegraphinsights-update.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Update the properties of a [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[List trending](../api/officegraphinsights-list-trending.md)|[trending](../resources/trending.md) collection|Get the trendings from the trending navigation property.|
|[Add trending](../api/officegraphinsights-post-trending.md)|[trending](../resources/trending.md)|Add trending by posting to the trending collection.|
|[List shared](../api/officegraphinsights-list-shared.md)|[sharedInsight](../resources/sharedinsight.md) collection|Get the sharedInsights from the shared navigation property.|
|[Add shared](../api/officegraphinsights-post-shared.md)|[sharedInsight](../resources/sharedinsight.md)|Add shared by posting to the shared collection.|
|[List used](../api/officegraphinsights-list-used.md)|[usedInsight](../resources/usedinsight.md) collection|Get the usedInsights from the used navigation property.|
|[Add used](../api/officegraphinsights-post-used.md)|[usedInsight](../resources/usedinsight.md)|Add used by posting to the used collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|shared|[sharedInsight](../resources/sharedinsight.md) collection||
|trending|[trending](../resources/trending.md) collection||
|used|[usedInsight](../resources/usedinsight.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeGraphInsights",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeGraphInsights",
  "id": "String (identifier)"
}
```

