---
title: "itemActivity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemActivity resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemActivity](../api/itemactivity-get.md)|[itemActivity](../resources/itemactivity.md)|Read properties and relationships of the [itemActivity](../resources/itemactivity.md) object.|
|[Update itemActivity](../api/itemactivity-update.md)|[itemActivity](../resources/itemactivity.md)|Update the properties of a [itemActivity](../resources/itemactivity.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[List activities](../api/itemactivitystat-list-activities.md)|[itemActivity](../resources/itemactivity.md) collection|Get the itemActivities from the activities navigation property.|
|[Create activities](../api/itemactivitystat-post-activities.md)|[itemActivity](../resources/itemactivity.md)|Create activities by posting to the activities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|access|[accessAction](../resources/accessaction.md)||
|activityDateTime|DateTimeOffset||
|actor|[identitySet](../resources/identityset.md)||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|driveItem|[driveItem](../resources/driveitem.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemActivity",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemActivity",
  "id": "String (identifier)",
  "access": {
    "@odata.type": "microsoft.graph.accessAction"
  },
  "activityDateTime": "String (timestamp)",
  "actor": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

