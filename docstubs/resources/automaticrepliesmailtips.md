---
title: "automaticRepliesMailTips resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# automaticRepliesMailTips resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String||
|messageLanguage|[localeInfo](../resources/localeinfo.md)||
|scheduledEndTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|scheduledStartTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.automaticRepliesMailTips",
  "message": "String",
  "messageLanguage": {
    "@odata.type": "microsoft.graph.localeInfo",
    "locale": "String",
    "displayName": "String"
  },
  "scheduledStartTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "scheduledEndTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

