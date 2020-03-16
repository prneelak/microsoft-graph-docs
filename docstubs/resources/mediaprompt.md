---
title: "mediaPrompt resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mediaPrompt resource type


Namespace: microsoft.graph




Inherits from [prompt](../resources/prompt.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|mediaInfo|[mediaInfo](../resources/mediainfo.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaPrompt"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "microsoft.graph.mediaInfo",
    "uri": "String",
    "resourceId": "String"
  }
}
```

