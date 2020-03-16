---
title: "pageLinks resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# pageLinks resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|oneNoteClientUrl|[externalLink](../resources/externallink.md)||
|oneNoteWebUrl|[externalLink](../resources/externallink.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pageLinks"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pageLinks",
  "oneNoteClientUrl": {
    "@odata.type": "microsoft.graph.externalLink",
    "href": "String"
  },
  "oneNoteWebUrl": {
    "@odata.type": "microsoft.graph.externalLink"
  }
}
```

