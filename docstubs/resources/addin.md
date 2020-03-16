---
title: "addIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# addIn resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|Guid||
|properties|[keyValue](../resources/keyvalue.md) collection||
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addIn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addIn",
  "id": "String (identifier)",
  "type": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ]
}
```

