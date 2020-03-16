---
title: "list resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# list resource type


Namespace: microsoft.graph




Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get list](../api/list-get.md)|[list](../resources/list.md)|Read properties and relationships of the [list](../resources/list.md) object.|
|[Update list](../api/list-update.md)|[list](../resources/list.md)|Update the properties of a [list](../resources/list.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[List columns](../api/list-list-columns.md)|[columnDefinition](../resources/columndefinition.md) collection|Get the columnDefinitions from the columns navigation property.|
|[Add columns](../api/list-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Add columns by posting to the columns collection.|
|[List contentTypes](../api/list-list-contenttypes.md)|[contentType](../resources/contenttype.md) collection|Get the contentTypes from the contentTypes navigation property.|
|[Add contentTypes](../api/list-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Add contentTypes by posting to the contentTypes collection.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read properties and relationships of the [drive](../resources/drive.md) object.|
|[List items](../api/list-list-items.md)|[listItem](../resources/listitem.md) collection|Get the listItems from the items navigation property.|
|[Add items](../api/list-post-items.md)|[listItem](../resources/listitem.md)|Add items by posting to the items collection.|
|[List lists](../api/site-list-lists.md)|[list](../resources/list.md) collection|Get the lists from the lists navigation property.|
|[Add lists](../api/site-post-lists.md)|[list](../resources/list.md)|Add lists by posting to the lists collection.|

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
|list|[listInfo](../resources/listinfo.md)||
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
|sharepointIds|[sharepointIds](../resources/sharepointids.md)||
|system|[systemFacet](../resources/systemfacet.md)||
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|columns|[columnDefinition](../resources/columndefinition.md) collection||
|contentTypes|[contentType](../resources/contenttype.md) collection||
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|drive|[drive](../resources/drive.md)||
|items|[listItem](../resources/listitem.md) collection||
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.list",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.list",
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
  "displayName": "String",
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "contentTypesEnabled": true,
    "hidden": true,
    "template": "String"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```

