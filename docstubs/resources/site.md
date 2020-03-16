---
title: "site resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# site resource type


Namespace: microsoft.graph




Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sites](../api/site-list.md)|[site](../resources/site.md) collection|List properties and relationships of the [site](../resources/site.md) objects.|
|[Get site](../api/site-get.md)|[site](../resources/site.md)|Read properties and relationships of the [site](../resources/site.md) object.|
|[Create site](../api/site-post-sites.md)|[site](../resources/site.md)|Create a new [site](../resources/site.md) object.|
|[Delete site](../api/site-delete.md)|None|Deletes a [site](../resources/site.md).|
|[Update site](../api/site-update.md)|[site](../resources/site.md)|Update the properties of a [site](../resources/site.md) object.|
|[getActivitiesByInterval](../api/site-getactivitiesbyinterval.md)|[itemActivityStat](../resources/itemactivitystat.md) collection||
|[getByPath](../api/site-getbypath.md)|[site](../resources/site.md)||
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemanalytics.md)|Read properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) object.|
|[List columns](../api/site-list-columns.md)|[columnDefinition](../resources/columndefinition.md) collection|Get the columnDefinitions from the columns navigation property.|
|[Add columns](../api/site-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Add columns by posting to the columns collection.|
|[List contentTypes](../api/site-list-contenttypes.md)|[contentType](../resources/contenttype.md) collection|Get the contentTypes from the contentTypes navigation property.|
|[Add contentTypes](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Add contentTypes by posting to the contentTypes collection.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read properties and relationships of the [drive](../resources/drive.md) object.|
|[List drives](../api/site-list-drives.md)|[drive](../resources/drive.md) collection|Get the drives from the drives navigation property.|
|[Add drives](../api/site-post-drives.md)|[drive](../resources/drive.md)|Add drives by posting to the drives collection.|
|[List items](../api/site-list-items.md)|[baseItem](../resources/baseitem.md) collection|Get the baseItems from the items navigation property.|
|[Add items](../api/site-post-items.md)|[baseItem](../resources/baseitem.md)|Add items by posting to the items collection.|
|[List lists](../api/site-list-lists.md)|[list](../resources/list.md) collection|Get the lists from the lists navigation property.|
|[Add lists](../api/site-post-lists.md)|[list](../resources/list.md)|Add lists by posting to the lists collection.|
|[List sites](../api/site-list-sites.md)|[site](../resources/site.md) collection|Get the sites from the sites navigation property.|
|[Add sites](../api/site-post-sites.md)|[site](../resources/site.md)|Add sites by posting to the sites collection.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read properties and relationships of the [onenote](../resources/onenote.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|description|String| Inherited from [baseItem](../resources/baseitem.md)|
|displayName|String||
|eTag|String| Inherited from [baseItem](../resources/baseitem.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
|root|[root](../resources/root.md)||
|sharepointIds|[sharepointIds](../resources/sharepointids.md)||
|siteCollection|[siteCollection](../resources/sitecollection.md)||
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|analytics|[itemAnalytics](../resources/itemanalytics.md)||
|columns|[columnDefinition](../resources/columndefinition.md) collection||
|contentTypes|[contentType](../resources/contenttype.md) collection||
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|drive|[drive](../resources/drive.md)||
|drives|[drive](../resources/drive.md) collection||
|items|[baseItem](../resources/baseitem.md) collection||
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lists|[list](../resources/list.md) collection||
|onenote|[onenote](../resources/onenote.md)||
|sites|[site](../resources/site.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.site",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.site",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
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
  "displayName": "String",
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "siteCollection": {
    "@odata.type": "microsoft.graph.siteCollection",
    "hostname": "String"
  }
}
```

