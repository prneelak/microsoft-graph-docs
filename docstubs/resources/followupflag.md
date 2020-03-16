---
title: "followupFlag resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# followupFlag resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|flagStatus|Enumeration|. Possible values are: `notFlagged`, `complete`, `flagged`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.followupFlag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.followupFlag",
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "flagStatus": "String"
}
```

