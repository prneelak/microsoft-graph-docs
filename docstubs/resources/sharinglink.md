---
title: "sharingLink resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharingLink resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|application|[identity](../resources/identity.md)||
|scope|String||
|type|String||
|webUrl|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharingLink"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharingLink",
  "application": {
    "@odata.type": "microsoft.graph.identity",
    "displayName": "String",
    "id": "String"
  },
  "scope": "String",
  "type": "String",
  "webUrl": "String"
}
```

