---
title: "fileEncryptionInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fileEncryptionInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|encryptionKey|Binary|The key used to encrypt the file content.|
|fileDigest|Binary|The file digest prior to encryption.|
|fileDigestAlgorithm|String|The file digest algorithm.|
|initializationVector|Binary|The initialization vector used for the encryption algorithm.|
|mac|Binary|The hash of the encrypted file content + IV (content hash).|
|macKey|Binary|The key used to get mac.|
|profileIdentifier|String|The the profile identifier.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```

