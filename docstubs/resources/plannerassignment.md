---
title: "plannerAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerAssignment resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedBy|[identitySet](../resources/identityset.md)||
|assignedDateTime|DateTimeOffset||
|orderHint|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerAssignment",
  "assignedBy": {
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
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}
```

