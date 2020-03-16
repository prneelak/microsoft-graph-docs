---
title: "plannerPlan resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerPlan resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerPlan](../api/plannerplan-get.md)|[plannerPlan](../resources/plannerplan.md)|Read properties and relationships of the [plannerPlan](../resources/plannerplan.md) object.|
|[Update plannerPlan](../api/plannerplan-update.md)|[plannerPlan](../resources/plannerplan.md)|Update the properties of a [plannerPlan](../resources/plannerplan.md) object.|
|[List tasks](../api/plannerplan-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/plannerplan-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Create tasks by posting to the tasks collection.|
|[List buckets](../api/plannerplan-list-buckets.md)|[plannerBucket](../resources/plannerbucket.md) collection|Get the plannerBuckets from the buckets navigation property.|
|[Create buckets](../api/plannerplan-post-buckets.md)|[plannerBucket](../resources/plannerbucket.md)|Create buckets by posting to the buckets collection.|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Read properties and relationships of the [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[List plans](../api/plannergroup-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Create plans](../api/plannergroup-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Create plans by posting to the plans collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|owner|String||
|title|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|buckets|[plannerBucket](../resources/plannerbucket.md) collection||
|details|[plannerPlanDetails](../resources/plannerplandetails.md)||
|tasks|[plannerTask](../resources/plannertask.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerPlan",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "String (timestamp)",
  "owner": "String",
  "title": "String"
}
```

