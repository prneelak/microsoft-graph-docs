---
title: "plannerUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerUser resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerUser](../api/planneruser-get.md)|[plannerUser](../resources/planneruser.md)|Read properties and relationships of the [plannerUser](../resources/planneruser.md) object.|
|[Update plannerUser](../api/planneruser-update.md)|[plannerUser](../resources/planneruser.md)|Update the properties of a [plannerUser](../resources/planneruser.md) object.|
|[List tasks](../api/planneruser-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/planneruser-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Create tasks by posting to the tasks collection.|
|[List plans](../api/planneruser-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Create plans](../api/planneruser-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Create plans by posting to the plans collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|plans|[plannerPlan](../resources/plannerplan.md) collection||
|tasks|[plannerTask](../resources/plannertask.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerUser",
  "id": "String (identifier)"
}
```

