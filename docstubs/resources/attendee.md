---
title: "attendee resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# attendee resource type


Namespace: microsoft.graph




Inherits from [attendeeBase](../resources/attendeebase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emailAddress|[emailAddress](../resources/emailaddress.md)| Inherited from [recipient](../resources/recipient.md)|
|status|[responseStatus](../resources/responsestatus.md)||
|type|Enumeration| Inherited from [attendeeBase](../resources/attendeebase.md). Possible values are: `required`, `optional`, `resource`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendee"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendee",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "String",
    "address": "String"
  },
  "type": "String",
  "status": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "String (timestamp)"
  }
}
```

