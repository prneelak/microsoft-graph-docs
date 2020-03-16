---
title: "fileSecurityState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fileSecurityState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|fileHash|[fileHash](../resources/filehash.md)||
|name|String||
|path|String||
|riskScore|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileSecurityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileSecurityState",
  "fileHash": {
    "@odata.type": "microsoft.graph.fileHash",
    "hashType": "String",
    "hashValue": "String"
  },
  "name": "String",
  "path": "String",
  "riskScore": "String"
}
```

