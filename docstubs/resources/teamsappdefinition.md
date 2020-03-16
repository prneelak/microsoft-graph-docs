---
title: "teamsAppDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsAppDefinition resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsAppDefinition](../api/teamsappdefinition-get.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Read properties and relationships of the [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[Update teamsAppDefinition](../api/teamsappdefinition-update.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Update the properties of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[List appDefinitions](../api/teamsapp-list-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md) collection|Get the teamsAppDefinitions from the appDefinitions navigation property.|
|[Add appDefinitions](../api/teamsapp-post-appdefinitions.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Add appDefinitions by posting to the appDefinitions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|teamsAppId|String||
|version|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "id": "String (identifier)",
  "teamsAppId": "String",
  "displayName": "String",
  "version": "String"
}
```

