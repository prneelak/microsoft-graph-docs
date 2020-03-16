---
title: "fileHash resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fileHash resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|hashType|Enumeration|. Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `unknownFutureValue`.|
|hashValue|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileHash"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileHash",
  "hashType": "String",
  "hashValue": "String"
}
```

