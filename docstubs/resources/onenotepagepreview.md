---
title: "onenotePagePreview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenotePagePreview resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|links|[onenotePagePreviewLinks](../resources/onenotepagepreviewlinks.md)||
|previewText|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onenotePagePreview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenotePagePreview",
  "previewText": "String",
  "links": {
    "@odata.type": "microsoft.graph.onenotePagePreviewLinks",
    "previewImageUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "String"
    }
  }
}
```

