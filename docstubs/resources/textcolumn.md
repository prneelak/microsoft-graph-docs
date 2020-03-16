---
title: "textColumn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# textColumn resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowMultipleLines|Boolean||
|appendChangesToExistingText|Boolean||
|linesForEditing|Int32||
|maxLength|Int32||
|textType|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.textColumn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.textColumn",
  "allowMultipleLines": true,
  "appendChangesToExistingText": true,
  "linesForEditing": 1024,
  "maxLength": 1024,
  "textType": "String"
}
```

