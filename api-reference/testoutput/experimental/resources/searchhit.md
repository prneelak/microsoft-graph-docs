---
title: "searchHit resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# searchHit resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|_id|String||
|_score|Int32||
|_sortField|String||
|_source|[entity](../resources/entity.md)||
|_summary|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchHit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchHit",
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": {
    "@odata.type": "#microsoft.graph.entity",
    "id": "String (identifier)"
  }
}
```

