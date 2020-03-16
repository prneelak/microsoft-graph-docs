---
title: "assignedPlan resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# assignedPlan resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedDateTime|DateTimeOffset||
|capabilityStatus|String||
|service|String||
|servicePlanId|Guid||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignedPlan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignedPlan",
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "String",
  "service": "String",
  "servicePlanId": "Guid"
}
```

