---
title: "plannerProgressTaskBoardTaskFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerProgressTaskBoardTaskFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)|Read properties and relationships of the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|
|[Update plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-update.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)|Update the properties of a [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHint|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "id": "String (identifier)",
  "orderHint": "String"
}
```

