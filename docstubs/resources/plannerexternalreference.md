---
title: "plannerExternalReference resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerExternalReference resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|alias|String||
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||
|previewPriority|String||
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerExternalReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerExternalReference",
  "alias": "String",
  "type": "String",
  "previewPriority": "String",
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

