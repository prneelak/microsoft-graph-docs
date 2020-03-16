---
title: "passwordCredential resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# passwordCredential resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|customKeyIdentifier|Binary||
|displayName|String||
|endDateTime|DateTimeOffset||
|hint|String||
|keyId|Guid||
|secretText|String||
|startDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordCredential"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordCredential",
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "secretText": "String",
  "hint": "String"
}
```

