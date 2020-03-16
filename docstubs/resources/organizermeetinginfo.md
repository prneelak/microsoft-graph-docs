---
title: "organizerMeetingInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# organizerMeetingInfo resource type


Namespace: microsoft.graph




Inherits from [meetingInfo](../resources/meetinginfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|organizer|[identitySet](../resources/identityset.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizerMeetingInfo",
  "organizer": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```

