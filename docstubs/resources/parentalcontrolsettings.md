---
title: "parentalControlSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# parentalControlSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|countriesBlockedForMinors|String collection||
|legalAgeGroupRule|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.parentalControlSettings",
  "countriesBlockedForMinors": [
    "String"
  ],
  "legalAgeGroupRule": "String"
}
```

