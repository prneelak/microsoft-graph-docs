---
title: "timeSlot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# timeSlot resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.timeSlot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeSlot",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

