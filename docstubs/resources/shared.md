---
title: "shared resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# shared resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|owner|[identitySet](../resources/identityset.md)||
|scope|String||
|sharedBy|[identitySet](../resources/identityset.md)||
|sharedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shared",
  "owner": {
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
  "scope": "String",
  "sharedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sharedDateTime": "String (timestamp)"
}
```

