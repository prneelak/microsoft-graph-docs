---
title: "managedAppOperation resource type"
description: "Represents an operation applied against an app registration."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppOperation resource type


Namespace: microsoft.graph

Represents an operation applied against an app registration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAppOperation](../api/managedappoperation-get.md)|[managedAppOperation](../resources/managedappoperation.md)|Read properties and relationships of the [managedAppOperation](../resources/managedappoperation.md) object.|
|[Update managedAppOperation](../api/managedappoperation-update.md)|[managedAppOperation](../resources/managedappoperation.md)|Update the properties of a [managedAppOperation](../resources/managedappoperation.md) object.|
|[List operations](../api/managedappregistration-list-operations.md)|[managedAppOperation](../resources/managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Add operations](../api/managedappregistration-post-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The operation name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The last time the app operation was modified.|
|state|String|The current state of the operation|
|version|String|Version of the entity.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```

