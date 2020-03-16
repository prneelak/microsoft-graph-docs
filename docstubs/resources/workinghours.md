---
title: "workingHours resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workingHours resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|daysOfWeek|Enumeration collection||
|endTime|TimeOfDay||
|startTime|TimeOfDay||
|timeZone|[timeZoneBase](../resources/timezonebase.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workingHours"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workingHours",
  "daysOfWeek": [
    "String"
  ],
  "startTime": "String (time of day)",
  "endTime": "String (time of day)",
  "timeZone": {
    "@odata.type": "microsoft.graph.timeZoneBase",
    "name": "String"
  }
}
```

