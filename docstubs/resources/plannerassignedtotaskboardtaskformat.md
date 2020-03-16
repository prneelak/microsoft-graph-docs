---
title: "plannerAssignedToTaskBoardTaskFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerAssignedToTaskBoardTaskFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Read properties and relationships of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Update plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-update.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Update the properties of a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](../resources/plannerorderhintsbyassignee.md)||
|unassignedOrderHint|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "id": "String (identifier)",
  "unassignedOrderHint": "String",
  "orderHintsByAssignee": {
    "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
  }
}
```

