---
title: "sharingDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharingDetail resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|sharedBy|[insightIdentity](../resources/insightidentity.md)||
|sharedDateTime|DateTimeOffset||
|sharingReference|[resourceReference](../resources/resourcereference.md)||
|sharingSubject|String||
|sharingType|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharingDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharingDetail",
  "sharedBy": {
    "@odata.type": "microsoft.graph.insightIdentity",
    "displayName": "String",
    "id": "String",
    "address": "String"
  },
  "sharedDateTime": "String (timestamp)",
  "sharingSubject": "String",
  "sharingType": "String",
  "sharingReference": {
    "@odata.type": "microsoft.graph.resourceReference",
    "webUrl": "String",
    "type": "String"
  }
}
```

