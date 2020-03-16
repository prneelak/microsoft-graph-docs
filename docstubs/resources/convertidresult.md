---
title: "convertIdResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# convertIdResult resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorDetails|[genericError](../resources/genericerror.md)||
|sourceId|String||
|targetId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.convertIdResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.convertIdResult",
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError",
    "message": "String",
    "code": "String"
  }
}
```

