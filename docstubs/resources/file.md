---
title: "file resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# file resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|hashes|[hashes](../resources/hashes.md)||
|mimeType|String||
|processingMetadata|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.file"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.file",
  "hashes": {
    "@odata.type": "microsoft.graph.hashes",
    "crc32Hash": "String",
    "quickXorHash": "String",
    "sha1Hash": "String"
  },
  "mimeType": "String",
  "processingMetadata": true
}
```

