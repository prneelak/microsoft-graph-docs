---
title: "mailboxSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mailboxSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|archiveFolder|String||
|automaticRepliesSetting|[automaticRepliesSetting](../resources/automaticrepliessetting.md)||
|dateFormat|String||
|language|[localeInfo](../resources/localeinfo.md)||
|timeFormat|String||
|timeZone|String||
|workingHours|[workingHours](../resources/workinghours.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailboxSettings",
  "automaticRepliesSetting": {
    "@odata.type": "microsoft.graph.automaticRepliesSetting",
    "status": "String",
    "externalAudience": "String",
    "scheduledStartDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "scheduledEndDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "internalReplyMessage": "String",
    "externalReplyMessage": "String"
  },
  "archiveFolder": "String",
  "timeZone": "String",
  "language": {
    "@odata.type": "microsoft.graph.localeInfo",
    "locale": "String",
    "displayName": "String"
  },
  "workingHours": {
    "@odata.type": "microsoft.graph.workingHours",
    "daysOfWeek": [
      "String"
    ],
    "startTime": "String (time of day)",
    "endTime": "String (time of day)",
    "timeZone": {
      "@odata.type": "microsoft.graph.timeZoneBase",
      "name": "String"
    }
  },
  "dateFormat": "String",
  "timeFormat": "String"
}
```

