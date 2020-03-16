---
title: "recurrencePattern resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# recurrencePattern resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|dayOfMonth|Int32||
|daysOfWeek|Enumeration collection||
|firstDayOfWeek|Enumeration|. Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|index|Enumeration|. Possible values are: `first`, `second`, `third`, `fourth`, `last`.|
|interval|Int32||
|month|Int32||
|type|Enumeration|. Possible values are: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly`, `relativeYearly`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recurrencePattern"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recurrencePattern",
  "type": "String",
  "interval": 1024,
  "month": 1024,
  "dayOfMonth": 1024,
  "daysOfWeek": [
    "String"
  ],
  "firstDayOfWeek": "String",
  "index": "String"
}
```

