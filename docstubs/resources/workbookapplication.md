---
title: "workbookApplication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookApplication resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookApplication](../api/workbookapplication-get.md)|[workbookApplication](../resources/workbookapplication.md)|Read properties and relationships of the [workbookApplication](../resources/workbookapplication.md) object.|
|[Update workbookApplication](../api/workbookapplication-update.md)|[workbookApplication](../resources/workbookapplication.md)|Update the properties of a [workbookApplication](../resources/workbookapplication.md) object.|
|[calculate](../api/workbookapplication-calculate.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calculationMode|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookApplication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookApplication",
  "id": "String (identifier)",
  "calculationMode": "String"
}
```

