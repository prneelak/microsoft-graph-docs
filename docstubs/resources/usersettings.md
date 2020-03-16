---
title: "userSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userSettings resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userSettings](../api/usersettings-get.md)|[userSettings](../resources/usersettings.md)|Read properties and relationships of the [userSettings](../resources/usersettings.md) object.|
|[Update userSettings](../api/usersettings-update.md)|[userSettings](../resources/usersettings.md)|Update the properties of a [userSettings](../resources/usersettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean||
|contributionToContentDiscoveryDisabled|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSettings",
  "id": "String (identifier)",
  "contributionToContentDiscoveryDisabled": true,
  "contributionToContentDiscoveryAsOrganizationDisabled": true
}
```

