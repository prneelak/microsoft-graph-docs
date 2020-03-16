---
title: "listItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# listItem resource type


Namespace: microsoft.graph




Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listitem.md)|Read properties and relationships of the [listItem](../resources/listitem.md) object.|
|[Update listItem](../api/listitem-update.md)|[listItem](../resources/listitem.md)|Update the properties of a [listItem](../resources/listitem.md) object.|
|[getActivitiesByInterval](../api/listitem-getactivitiesbyinterval.md)|[itemActivityStat](../resources/itemactivitystat.md) collection||
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemanalytics.md)|Read properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[Get fieldValueSet](../api/fieldvalueset-get.md)|[fieldValueSet](../resources/fieldvalueset.md)|Read properties and relationships of the [fieldValueSet](../resources/fieldvalueset.md) object.|
|[List versions](../api/listitem-list-versions.md)|[listItemVersion](../resources/listitemversion.md) collection|Get the listItemVersions from the versions navigation property.|
|[Add versions](../api/listitem-post-versions.md)|[listItemVersion](../resources/listitemversion.md)|Add versions by posting to the versions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentType|[contentTypeInfo](../resources/contenttypeinfo.md)||
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|description|String| Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseitem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)||
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|analytics|[itemAnalytics](../resources/itemanalytics.md)||
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|driveItem|[driveItem](../resources/driveitem.md)||
|fields|[fieldValueSet](../resources/fieldvalueset.md)||
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|versions|[listItemVersion](../resources/listitemversion.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.listItem",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.listItem",
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
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "String",
    "driveType": "String",
    "path": "String",
    "shareId": "String",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "String",
      "listItemId": "String",
      "listItemUniqueId": "String",
      "siteId": "String",
      "siteUrl": "String",
      "webId": "String"
    }
  },
  "webUrl": "String",
  "contentType": {
    "@odata.type": "microsoft.graph.contentTypeInfo"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  }
}
```

