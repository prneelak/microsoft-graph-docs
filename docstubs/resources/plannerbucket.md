---
title: "plannerBucket resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerBucket resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerBucket](../api/plannerbucket-get.md)|[plannerBucket](../resources/plannerbucket.md)|Read properties and relationships of the [plannerBucket](../resources/plannerbucket.md) object.|
|[Update plannerBucket](../api/plannerbucket-update.md)|[plannerBucket](../resources/plannerbucket.md)|Update the properties of a [plannerBucket](../resources/plannerbucket.md) object.|
|[List tasks](../api/plannerbucket-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/plannerbucket-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Create tasks by posting to the tasks collection.|
|[List buckets](../api/plannerplan-list-buckets.md)|[plannerBucket](../resources/plannerbucket.md) collection|Get the plannerBuckets from the buckets navigation property.|
|[Create buckets](../api/plannerplan-post-buckets.md)|[plannerBucket](../resources/plannerbucket.md)|Create buckets by posting to the buckets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|orderHint|String||
|planId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|tasks|[plannerTask](../resources/plannertask.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerBucket",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "id": "String (identifier)",
  "name": "String",
  "planId": "String",
  "orderHint": "String"
}
```

