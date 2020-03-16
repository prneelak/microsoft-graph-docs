---
title: "appCatalogs resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appCatalogs resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appCatalogs](../api/appcatalogs-get.md)|[appCatalogs](../resources/appcatalogs.md)|Read properties and relationships of the [appCatalogs](../resources/appcatalogs.md) object.|
|[Update appCatalogs](../api/appcatalogs-update.md)|[appCatalogs](../resources/appcatalogs.md)|Update the properties of a [appCatalogs](../resources/appcatalogs.md) object.|
|[List teamsApps](../api/appcatalogs-list-teamsapps.md)|[teamsApp](../resources/teamsapp.md) collection|Get the teamsApps from the teamsApps navigation property.|
|[Add teamsApps](../api/appcatalogs-post-teamsapps.md)|[teamsApp](../resources/teamsapp.md)|Add teamsApps by posting to the teamsApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApps|[teamsApp](../resources/teamsapp.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appCatalogs",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appCatalogs",
  "id": "String (identifier)"
}
```

