---
title: "sharedDriveItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharedDriveItem resource type


Namespace: microsoft.graph




Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharedDriveItems](../api/shareddriveitem-list.md)|[sharedDriveItem](../resources/shareddriveitem.md) collection|List properties and relationships of the [sharedDriveItem](../resources/shareddriveitem.md) objects.|
|[Get sharedDriveItem](../api/shareddriveitem-get.md)|[sharedDriveItem](../resources/shareddriveitem.md)|Read properties and relationships of the [sharedDriveItem](../resources/shareddriveitem.md) object.|
|[Create sharedDriveItem](../api/shareddriveitem-post-shares.md)|[sharedDriveItem](../resources/shareddriveitem.md)|Create a new [sharedDriveItem](../resources/shareddriveitem.md) object.|
|[Delete sharedDriveItem](../api/shareddriveitem-delete.md)|None|Deletes a [sharedDriveItem](../resources/shareddriveitem.md).|
|[Update sharedDriveItem](../api/shareddriveitem-update.md)|[sharedDriveItem](../resources/shareddriveitem.md)|Update the properties of a [sharedDriveItem](../resources/shareddriveitem.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[List items](../api/shareddriveitem-list-items.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the items navigation property.|
|[Add items](../api/shareddriveitem-post-items.md)|[driveItem](../resources/driveitem.md)|Add items by posting to the items collection.|
|[Get list](../api/list-get.md)|[list](../resources/list.md)|Read properties and relationships of the [list](../resources/list.md) object.|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listitem.md)|Read properties and relationships of the [listItem](../resources/listitem.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[Get site](../api/site-get.md)|[site](../resources/site.md)|Read properties and relationships of the [site](../resources/site.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|description|String| Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseitem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|owner|[identitySet](../resources/identityset.md)||
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|driveItem|[driveItem](../resources/driveitem.md)||
|items|[driveItem](../resources/driveitem.md) collection||
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|list|[list](../resources/list.md)||
|listItem|[listItem](../resources/listitem.md)||
|root|[driveItem](../resources/driveitem.md)||
|site|[site](../resources/site.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedDriveItem",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedDriveItem",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

