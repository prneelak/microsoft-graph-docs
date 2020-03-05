---
title: "teamsTab resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsTab resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsTabs](../api/teamstab-list.md)|[teamsTab](../resources/teamstab.md) collection|List properties and relationships of the [teamsTab](../resources/teamstab.md) objects.|
|[Get teamsTab](../api/teamstab-get.md)|[teamsTab](../resources/teamstab.md)|Read properties and relationships of the [teamsTab](../resources/teamstab.md) object.|
|[Create teamsTab](../api/teamstab-create.md)|[teamsTab](../resources/teamstab.md)|Create a new [teamsTab](../resources/teamstab.md) object.|
|[Delete teamsTab](../api/teamstab-delete.md)|None|Deletes a [teamsTab](../resources/teamstab.md).|
|[Update teamsTab](../api/teamstab-update.md)|[teamsTab](../resources/teamstab.md)|Update the properties of a [teamsTab](../resources/teamstab.md) object.|
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsapp.md)|Read properties and relationships of the [teamsApp](../resources/teamsapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configuration|[teamsTabConfiguration](../resources/teamstabconfiguration.md)||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|webUrl|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApp|[teamsApp](../resources/teamsapp.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsTab",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsTab",
  "id": "String (identifier)",
  "displayName": "String",
  "webUrl": "String",
  "configuration": {
    "@odata.type": "microsoft.graph.teamsTabConfiguration",
    "entityId": "String",
    "contentUrl": "String",
    "removeUrl": "String",
    "websiteUrl": "String"
  }
}
```

