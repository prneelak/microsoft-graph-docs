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
|[List plannerAssignedToTaskBoardTaskFormats](../api/plannerassignedtotaskboardtaskformat-list.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) collection|List properties and relationships of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) objects.|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Read properties and relationships of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Create plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-create.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Create a new [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Delete plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-delete.md)|None|Deletes a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md).|
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

