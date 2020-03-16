---
title: "plannerChecklistItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerChecklistItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|isChecked|Boolean||
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||
|orderHint|String||
|title|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerChecklistItem",
  "isChecked": true,
  "title": "String",
  "orderHint": "String",
  "lastModifiedBy": {
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
  "lastModifiedDateTime": "String (timestamp)"
}
```

