---
title: "workbookFilterCriteria resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookFilterCriteria resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String||
|criterion1|String||
|criterion2|String||
|dynamicCriteria|String||
|filterOn|String||
|icon|[workbookIcon](../resources/workbookicon.md)||
|operator|String||
|values|[Json](../resources/json.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFilterCriteria",
  "color": "String",
  "criterion1": "String",
  "criterion2": "String",
  "dynamicCriteria": "String",
  "filterOn": "String",
  "icon": {
    "@odata.type": "microsoft.graph.workbookIcon",
    "index": 1024,
    "set": "String"
  },
  "operator": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

