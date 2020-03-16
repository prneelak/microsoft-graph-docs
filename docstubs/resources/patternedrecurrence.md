---
title: "patternedRecurrence resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# patternedRecurrence resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|pattern|[recurrencePattern](../resources/recurrencepattern.md)||
|range|[recurrenceRange](../resources/recurrencerange.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.patternedRecurrence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.patternedRecurrence",
  "pattern": {
    "@odata.type": "microsoft.graph.recurrencePattern",
    "type": "String",
    "interval": 1024,
    "month": 1024,
    "dayOfMonth": 1024,
    "daysOfWeek": [
      "String"
    ],
    "firstDayOfWeek": "String",
    "index": "String"
  },
  "range": {
    "@odata.type": "microsoft.graph.recurrenceRange",
    "type": "String",
    "startDate": "Date",
    "endDate": "Date",
    "recurrenceTimeZone": "String",
    "numberOfOccurrences": 1024
  }
}
```

