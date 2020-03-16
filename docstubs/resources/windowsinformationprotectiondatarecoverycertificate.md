---
title: "windowsInformationProtectionDataRecoveryCertificate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionDataRecoveryCertificate resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificate|Binary|Data recovery Certificate|
|description|String|Data recovery Certificate description|
|expirationDateTime|DateTimeOffset|Data recovery Certificate expiration datetime|
|subjectName|String|Data recovery Certificate subject name|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```

