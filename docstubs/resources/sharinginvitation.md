---
title: "sharingInvitation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharingInvitation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|email|String||
|invitedBy|[identitySet](../resources/identityset.md)||
|redeemedBy|String||
|signInRequired|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharingInvitation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharingInvitation",
  "email": "String",
  "invitedBy": {
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
  "redeemedBy": "String",
  "signInRequired": true
}
```

