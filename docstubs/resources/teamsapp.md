---
title: "teamsApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsApp resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsapp.md)|Read properties and relationships of the [teamsApp](../resources/teamsapp.md) object.|
|[Update teamsApp](../api/teamsapp-update.md)|[teamsApp](../resources/teamsapp.md)|Update the properties of a [teamsApp](../resources/teamsapp.md) object.|
|[List appDefinitions](../api/teamsapp-list-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md) collection|Get the teamsAppDefinitions from the appDefinitions navigation property.|
|[Add appDefinitions](../api/teamsapp-post-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Add appDefinitions by posting to the appDefinitions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|distributionMethod|Enumeration|. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|
|externalId|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appDefinitions|[teamsAppDefinition](../resources/teamsappdefinition.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsApp",
  "id": "String (identifier)",
  "externalId": "String",
  "displayName": "String",
  "distributionMethod": "String"
}
```

