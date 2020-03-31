---
title: "teamsCatalogApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsCatalogApp resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsCatalogApp](../api/teamscatalogapp-get.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Read properties and relationships of the [teamsCatalogApp](../resources/teamscatalogapp.md) object.|
|[Update teamsCatalogApp](../api/teamscatalogapp-update.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Update the properties of a [teamsCatalogApp](../resources/teamscatalogapp.md) object.|
|[List apps](../api/team-list-apps.md)|[teamsCatalogApp](../resources/teamscatalogapp.md) collection|Get the teamsCatalogApps from the apps navigation property.|
|[Add apps](../api/team-post-apps.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Add apps by posting to the apps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|distributionMethod|Enumeration| Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|
|externalId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsCatalogApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "id": "String (identifier)",
  "externalId": "String",
  "name": "String",
  "distributionMethod": "String"
}
```

