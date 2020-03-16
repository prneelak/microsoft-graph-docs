---
title: "onenotePatchContentCommand resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenotePatchContentCommand resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|Enumeration|. Possible values are: `Replace`, `Append`, `Delete`, `Insert`, `Prepend`.|
|content|String||
|position|Enumeration|. Possible values are: `After`, `Before`.|
|target|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenotePatchContentCommand",
  "action": "String",
  "target": "String",
  "content": "String",
  "position": "String"
}
```

