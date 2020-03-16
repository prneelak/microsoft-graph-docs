---
title: "teamFunSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamFunSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowCustomMemes|Boolean||
|allowGiphy|Boolean||
|allowStickersAndMemes|Boolean||
|giphyContentRating|Enumeration|. Possible values are: `moderate`, `strict`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamFunSettings",
  "allowGiphy": true,
  "giphyContentRating": "String",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

