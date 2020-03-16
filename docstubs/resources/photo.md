---
title: "photo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# photo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|cameraMake|String||
|cameraModel|String||
|exposureDenominator|Double||
|exposureNumerator|Double||
|fNumber|Double||
|focalLength|Double||
|iso|Int32||
|takenDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.photo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.photo",
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": "Double",
  "exposureNumerator": "Double",
  "fNumber": "Double",
  "focalLength": "Double",
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

