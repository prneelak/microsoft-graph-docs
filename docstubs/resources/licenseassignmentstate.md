---
title: "licenseAssignmentState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# licenseAssignmentState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedByGroup|String||
|disabledPlans|Guid collection||
|error|String||
|skuId|Guid||
|state|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.licenseAssignmentState",
  "skuId": "Guid",
  "disabledPlans": [
    "Guid"
  ],
  "assignedByGroup": "String",
  "state": "String",
  "error": "String"
}
```

