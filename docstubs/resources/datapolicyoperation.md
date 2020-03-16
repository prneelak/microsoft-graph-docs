---
title: "dataPolicyOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dataPolicyOperation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List dataPolicyOperations](../api/datapolicyoperation-list.md)|[dataPolicyOperation](../resources/datapolicyoperation.md) collection|List properties and relationships of the [dataPolicyOperation](../resources/datapolicyoperation.md) objects.|
|[Get dataPolicyOperation](../api/datapolicyoperation-get.md)|[dataPolicyOperation](../resources/datapolicyoperation.md)|Read properties and relationships of the [dataPolicyOperation](../resources/datapolicyoperation.md) object.|
|[Create dataPolicyOperation](../api/datapolicyoperation-post-datapolicyoperations.md)|[dataPolicyOperation](../resources/datapolicyoperation.md)|Create a new [dataPolicyOperation](../resources/datapolicyoperation.md) object.|
|[Delete dataPolicyOperation](../api/datapolicyoperation-delete.md)|None|Deletes a [dataPolicyOperation](../resources/datapolicyoperation.md).|
|[Update dataPolicyOperation](../api/datapolicyoperation-update.md)|[dataPolicyOperation](../resources/datapolicyoperation.md)|Update the properties of a [dataPolicyOperation](../resources/datapolicyoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|progress|Double||
|status|Enumeration|. Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String||
|submittedDateTime|DateTimeOffset||
|userId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataPolicyOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "id": "String (identifier)",
  "completedDateTime": "String (timestamp)",
  "status": "String",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
}
```

