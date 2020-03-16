---
title: "planner resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# planner resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get planner](../api/planner-get.md)|[planner](../resources/planner.md)|Read properties and relationships of the [planner](../resources/planner.md) object.|
|[Update planner](../api/planner-update.md)|[planner](../resources/planner.md)|Update the properties of a [planner](../resources/planner.md) object.|
|[List tasks](../api/planner-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Add tasks](../api/planner-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Add tasks by posting to the tasks collection.|
|[List plans](../api/planner-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Add plans](../api/planner-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Add plans by posting to the plans collection.|
|[List buckets](../api/planner-list-buckets.md)|[plannerBucket](../resources/plannerbucket.md) collection|Get the plannerBuckets from the buckets navigation property.|
|[Add buckets](../api/planner-post-buckets.md)|[plannerBucket](../resources/plannerbucket.md)|Add buckets by posting to the buckets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|buckets|[plannerBucket](../resources/plannerbucket.md) collection||
|plans|[plannerPlan](../resources/plannerplan.md) collection||
|tasks|[plannerTask](../resources/plannertask.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.planner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.planner",
  "id": "String (identifier)"
}
```

