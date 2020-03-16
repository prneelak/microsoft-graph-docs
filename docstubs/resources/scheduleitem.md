---
title: "scheduleItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# scheduleItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|isPrivate|Boolean||
|location|String||
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|status|Enumeration|. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|subject|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scheduleItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scheduleItem",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "isPrivate": true,
  "status": "String",
  "subject": "String",
  "location": "String"
}
```

