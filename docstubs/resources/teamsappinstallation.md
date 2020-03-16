---
title: "teamsAppInstallation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsAppInstallation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsAppInstallation](../api/teamsappinstallation-get.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Read properties and relationships of the [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[Update teamsAppInstallation](../api/teamsappinstallation-update.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Update the properties of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[upgrade](../api/teamsappinstallation-upgrade.md)|None||
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsapp.md)|Read properties and relationships of the [teamsApp](../resources/teamsapp.md) object.|
|[Get teamsAppDefinition](../api/teamsappdefinition-get.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Read properties and relationships of the [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[List installedApps](../api/team-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Add installedApps](../api/team-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Add installedApps by posting to the installedApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApp|[teamsApp](../resources/teamsapp.md)||
|teamsAppDefinition|[teamsAppDefinition](../resources/teamsappdefinition.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppInstallation",
  "id": "String (identifier)"
}
```

