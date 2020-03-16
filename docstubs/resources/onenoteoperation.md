---
title: "onenoteOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenoteOperation resource type


Namespace: microsoft.graph




Inherits from [operation](../resources/operation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenoteOperation](../api/onenoteoperation-get.md)|[onenoteOperation](../resources/onenoteoperation.md)|Read properties and relationships of the [onenoteOperation](../resources/onenoteoperation.md) object.|
|[Update onenoteOperation](../api/onenoteoperation-update.md)|[onenoteOperation](../resources/onenoteoperation.md)|Update the properties of a [onenoteOperation](../resources/onenoteoperation.md) object.|
|[List operations](../api/onenote-list-operations.md)|[onenoteOperation](../resources/onenoteoperation.md) collection|Get the onenoteOperations from the operations navigation property.|
|[Add operations](../api/onenote-post-operations.md)|[onenoteOperation](../resources/onenoteoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|error|[onenoteOperationError](../resources/onenoteoperationerror.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActionDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|percentComplete|String||
|resourceId|String||
|resourceLocation|String||
|status|Enumeration| Inherited from [operation](../resources/operation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteOperation",
  "baseType": "microsoft.graph.operation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "id": "String (identifier)",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "resourceId": "String",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError"
  },
  "percentComplete": "String"
}
```

