---
title: "itemAnalytics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemAnalytics resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemanalytics.md)|Read properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) object.|
|[Update itemAnalytics](../api/itemanalytics-update.md)|[itemAnalytics](../resources/itemanalytics.md)|Update the properties of a [itemAnalytics](../resources/itemanalytics.md) object.|
|[List itemActivityStats](../api/itemanalytics-list-itemactivitystats.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|Get the itemActivityStats from the itemActivityStats navigation property.|
|[Add itemActivityStats](../api/itemanalytics-post-itemactivitystats.md)|[itemActivityStat](../resources/itemactivitystat.md)|Add itemActivityStats by posting to the itemActivityStats collection.|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemactivitystat.md)|Read properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemactivitystat.md)|Read properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|allTime|[itemActivityStat](../resources/itemactivitystat.md)||
|itemActivityStats|[itemActivityStat](../resources/itemactivitystat.md) collection||
|lastSevenDays|[itemActivityStat](../resources/itemactivitystat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAnalytics",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAnalytics",
  "id": "String (identifier)"
}
```

