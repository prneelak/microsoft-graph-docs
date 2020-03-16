---
title: "workbookSortField resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookSortField resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|ascending|Boolean||
|color|String||
|dataOption|String||
|icon|[workbookIcon](../resources/workbookicon.md)||
|key|Int32||
|sortOn|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workbookSortField"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookSortField",
  "ascending": true,
  "color": "String",
  "dataOption": "String",
  "icon": {
    "@odata.type": "microsoft.graph.workbookIcon",
    "index": 1024,
    "set": "String"
  },
  "key": 1024,
  "sortOn": "String"
}
```

