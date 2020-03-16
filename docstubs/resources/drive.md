---
title: "drive resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# drive resource type


Namespace: microsoft.graph




Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List drives](../api/drive-list.md)|[drive](../resources/drive.md) collection|List properties and relationships of the [drive](../resources/drive.md) objects.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read properties and relationships of the [drive](../resources/drive.md) object.|
|[Create drive](../api/drive-post-drives.md)|[drive](../resources/drive.md)|Create a new [drive](../resources/drive.md) object.|
|[Delete drive](../api/drive-delete.md)|None|Deletes a [drive](../resources/drive.md).|
|[Update drive](../api/drive-update.md)|[drive](../resources/drive.md)|Update the properties of a [drive](../resources/drive.md) object.|
|[recent](../api/drive-recent.md)|[driveItem](../resources/driveitem.md) collection||
|[search](../api/drive-search.md)|[driveItem](../resources/driveitem.md) collection||
|[sharedWithMe](../api/drive-sharedwithme.md)|[driveItem](../resources/driveitem.md) collection||
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[List items](../api/drive-list-items.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the items navigation property.|
|[Add items](../api/drive-post-items.md)|[driveItem](../resources/driveitem.md)|Add items by posting to the items collection.|
|[Get list](../api/list-get.md)|[list](../resources/list.md)|Read properties and relationships of the [list](../resources/list.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[List special](../api/drive-list-special.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the special navigation property.|
|[Add special](../api/drive-post-special.md)|[driveItem](../resources/driveitem.md)|Add special by posting to the special collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|description|String| Inherited from [baseItem](../resources/baseitem.md)|
|driveType|String||
|eTag|String| Inherited from [baseItem](../resources/baseitem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|owner|[identitySet](../resources/identityset.md)||
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
|quota|[quota](../resources/quota.md)||
|sharePointIds|[sharepointIds](../resources/sharepointids.md)||
|system|[systemFacet](../resources/systemfacet.md)||
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|items|[driveItem](../resources/driveitem.md) collection||
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|list|[list](../resources/list.md)||
|root|[driveItem](../resources/driveitem.md)||
|special|[driveItem](../resources/driveitem.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.drive",
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
  "driveType": "String",
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "quota": {
    "@odata.type": "microsoft.graph.quota",
    "deleted": 1024,
    "remaining": 1024,
    "total": 1024,
    "used": 1024
  },
  "sharePointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```

