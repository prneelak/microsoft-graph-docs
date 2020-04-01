---
title: "attendee resource type"
description: "An event attendee. This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant."
localization_priority: Normal
author: ""
ms.prod: ""
doc_type: resourcePageType
---

# attendee resource type

Namespace: microsoft.graph

An event attendee. This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.

Derived from [attendeeBase](attendeebase.md).

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|status|[ResponseStatus](responsestatus.md)|The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.|
|type|String|The attendee type: `required`, `optional`, `resource`.|
|emailAddress|[emailAddress](emailaddress.md)|Includes the name and SMTP address of the attendee.|

## JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
