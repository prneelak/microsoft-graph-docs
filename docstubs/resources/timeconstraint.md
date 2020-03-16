---
title: "timeConstraint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# timeConstraint resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityDomain|Enumeration|. Possible values are: `unknown`, `work`, `personal`, `unrestricted`.|
|timeSlots|[timeSlot](../resources/timeslot.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.timeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeConstraint",
  "activityDomain": "String",
  "timeSlots": [
    {
      "@odata.type": "microsoft.graph.timeSlot",
      "start": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone",
        "dateTime": "String",
        "timeZone": "String"
      },
      "end": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      }
    }
  ]
}
```

