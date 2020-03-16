---
title: "scoredEmailAddress resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# scoredEmailAddress resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String||
|itemId|String||
|relevanceScore|Double||
|selectionLikelihood|Enumeration|. Possible values are: `notSpecified`, `high`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scoredEmailAddress",
  "address": "String",
  "relevanceScore": "Double",
  "selectionLikelihood": "String",
  "itemId": "String"
}
```

