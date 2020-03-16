---
title: "commsOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# commsOperation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get commsOperation](../api/commsoperation-get.md)|[commsOperation](../resources/commsoperation.md)|Read properties and relationships of the [commsOperation](../resources/commsoperation.md) object.|
|[Update commsOperation](../api/commsoperation-update.md)|[commsOperation](../resources/commsoperation.md)|Update the properties of a [commsOperation](../resources/commsoperation.md) object.|
|[List operations](../api/call-list-operations.md)|[commsOperation](../resources/commsoperation.md) collection|Get the commsOperations from the operations navigation property.|
|[Add operations](../api/call-post-operations.md)|[commsOperation](../resources/commsoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resultInfo|[resultInfo](../resources/resultinfo.md)||
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.commsOperation",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.commsOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```

