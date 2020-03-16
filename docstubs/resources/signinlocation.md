---
title: "signInLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# signInLocation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String||
|countryOrRegion|String||
|geoCoordinates|[geoCoordinates](../resources/geocoordinates.md)||
|state|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.signInLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signInLocation",
  "city": "String",
  "state": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  }
}
```

