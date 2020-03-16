---
title: "itemReference resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemReference resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|driveId|String||
|driveType|String||
|id|String||
|name|String||
|path|String||
|shareId|String||
|sharepointIds|[sharepointIds](../resources/sharepointids.md)||
|siteId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.itemReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemReference",
  "driveId": "String",
  "driveType": "String",
  "id": "String (identifier)",
  "name": "String",
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
  },
  "siteId": "String"
}
```

