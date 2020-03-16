---
title: "plannerGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerGroup resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerGroup](../api/plannergroup-get.md)|[plannerGroup](../resources/plannergroup.md)|Read properties and relationships of the [plannerGroup](../resources/plannergroup.md) object.|
|[Update plannerGroup](../api/plannergroup-update.md)|[plannerGroup](../resources/plannergroup.md)|Update the properties of a [plannerGroup](../resources/plannergroup.md) object.|
|[List plans](../api/plannergroup-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Create plans](../api/plannergroup-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Create plans by posting to the plans collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|plans|[plannerPlan](../resources/plannerplan.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerGroup",
  "id": "String (identifier)"
}
```

