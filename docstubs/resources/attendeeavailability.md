---
title: "attendeeAvailability resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# attendeeAvailability resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendee|[attendeeBase](../resources/attendeebase.md)||
|availability|Enumeration|. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendeeAvailability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendeeAvailability",
  "attendee": {
    "@odata.type": "microsoft.graph.attendeeBase",
    "emailAddress": {
      "@odata.type": "microsoft.graph.emailAddress",
      "name": "String",
      "address": "String"
    },
    "type": "String"
  },
  "availability": "String"
}
```

