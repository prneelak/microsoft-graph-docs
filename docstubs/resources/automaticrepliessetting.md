---
title: "automaticRepliesSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# automaticRepliesSetting resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|externalAudience|Enumeration|. Possible values are: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|String||
|internalReplyMessage|String||
|scheduledEndDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|scheduledStartDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|status|Enumeration|. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.automaticRepliesSetting",
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
}
```

