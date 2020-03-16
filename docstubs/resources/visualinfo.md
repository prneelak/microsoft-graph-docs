---
title: "visualInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# visualInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attribution|[imageInfo](../resources/imageinfo.md)||
|backgroundColor|String||
|content|[Json](../resources/json.md)||
|description|String||
|displayText|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.visualInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.visualInfo",
  "attribution": {
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String",
    "alternativeText": "String",
    "alternateText": "String",
    "addImageQuery": true
  },
  "backgroundColor": "String",
  "description": "String",
  "displayText": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

