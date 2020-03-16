---
title: "uploadSession resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# uploadSession resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset||
|nextExpectedRanges|String collection||
|uploadUrl|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.uploadSession",
  "expirationDateTime": "String (timestamp)",
  "nextExpectedRanges": [
    "String"
  ],
  "uploadUrl": "String"
}
```

