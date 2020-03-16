---
title: "certificateAuthority resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# certificateAuthority resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificate|Binary||
|certificateRevocationListUrl|String||
|deltaCertificateRevocationListUrl|String||
|isRootAuthority|Boolean||
|issuer|String||
|issuerSki|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateAuthority"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateAuthority",
  "isRootAuthority": true,
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "certificate": "binary",
  "issuer": "String",
  "issuerSki": "String"
}
```

