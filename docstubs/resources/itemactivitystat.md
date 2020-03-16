---
title: "itemActivityStat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemActivityStat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemactivitystat.md)|Read properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Update itemActivityStat](../api/itemactivitystat-update.md)|[itemActivityStat](../resources/itemactivitystat.md)|Update the properties of a [itemActivityStat](../resources/itemactivitystat.md) object.|
|[List activities](../api/itemactivitystat-list-activities.md)|[itemActivity](../resources/itemactivity.md) collection|Get the itemActivities from the activities navigation property.|
|[Create activities](../api/itemactivitystat-post-activities.md)|[itemActivity](../resources/itemactivity.md)|Create activities by posting to the activities collection.|
|[List itemActivityStats](../api/itemanalytics-list-itemactivitystats.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|Get the itemActivityStats from the itemActivityStats navigation property.|
|[Add itemActivityStats](../api/itemanalytics-post-itemactivitystats.md)|[itemActivityStat](../resources/itemactivitystat.md)|Add itemActivityStats by posting to the itemActivityStats collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|access|[itemActionStat](../resources/itemactionstat.md)||
|create|[itemActionStat](../resources/itemactionstat.md)||
|delete|[itemActionStat](../resources/itemactionstat.md)||
|edit|[itemActionStat](../resources/itemactionstat.md)||
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|incompleteData|[incompleteData](../resources/incompletedata.md)||
|isTrending|Boolean||
|move|[itemActionStat](../resources/itemactionstat.md)||
|startDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivity](../resources/itemactivity.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemActivityStat",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "access": {
    "@odata.type": "microsoft.graph.itemActionStat",
    "actionCount": 1024,
    "actorCount": 1024
  },
  "create": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "delete": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "edit": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "move": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "isTrending": true,
  "incompleteData": {
    "@odata.type": "microsoft.graph.incompleteData",
    "missingDataBeforeDateTime": "String (timestamp)",
    "wasThrottled": true
  }
}
```

