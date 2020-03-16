---
title: "audio resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# audio resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|album|String||
|albumArtist|String||
|artist|String||
|bitrate|Int64||
|composers|String||
|copyright|String||
|disc|Int16||
|discCount|Int16||
|duration|Int64||
|genre|String||
|hasDrm|Boolean||
|isVariableBitrate|Boolean||
|title|String||
|track|Int32||
|trackCount|Int32||
|year|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.audio"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.audio",
  "album": "String",
  "albumArtist": "String",
  "artist": "String",
  "bitrate": 1024,
  "composers": "String",
  "copyright": "String",
  "disc": 1024,
  "discCount": 1024,
  "duration": 1024,
  "genre": "String",
  "hasDrm": true,
  "isVariableBitrate": true,
  "title": "String",
  "track": 1024,
  "trackCount": 1024,
  "year": 1024
}
```

