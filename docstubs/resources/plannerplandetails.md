---
title: "plannerPlanDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerPlanDetails resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Read properties and relationships of the [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Update plannerPlanDetails](../api/plannerplandetails-update.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Update the properties of a [plannerPlanDetails](../resources/plannerplandetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerPlanDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "String (identifier)",
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  },
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
  }
}
```

