---
title: "invitationParticipantInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# invitationParticipantInfo resource type


Namespace: microsoft.graph




Inherits from [participantInfo](../resources/participantinfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|identity|[identitySet](../resources/identityset.md)| Inherited from [participantInfo](../resources/participantinfo.md)|
|languageId|String| Inherited from [participantInfo](../resources/participantinfo.md)|
|region|String| Inherited from [participantInfo](../resources/participantinfo.md)|
|replacesCallId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.invitationParticipantInfo",
  "identity": {
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
  },
  "region": "String",
  "languageId": "String",
  "replacesCallId": "String"
}
```

