---
title: "keyCredential resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# keyCredential resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|customKeyIdentifier|Binary||
|displayName|String||
|endDateTime|DateTimeOffset||
|key|Binary||
|keyId|Guid||
|startDateTime|DateTimeOffset||
|type|String||
|usage|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyCredential"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyCredential",
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String",
  "key": "binary"
}
```

