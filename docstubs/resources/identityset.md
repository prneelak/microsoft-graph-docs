---
title: "identitySet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# identitySet resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|application|[identity](../resources/identity.md)||
|device|[identity](../resources/identity.md)||
|user|[identity](../resources/identity.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identitySet",
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
```

