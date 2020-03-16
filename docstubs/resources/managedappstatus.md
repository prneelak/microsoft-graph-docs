---
title: "managedAppStatus resource type"
description: "Represents app protection and configuration status for the organization."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppStatus resource type


Namespace: microsoft.graph

Represents app protection and configuration status for the organization.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAppStatus](../api/managedappstatus-get.md)|[managedAppStatus](../resources/managedappstatus.md)|Read properties and relationships of the [managedAppStatus](../resources/managedappstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Friendly name of the status report.|
|id|String| Inherited from [entity](../resources/entity.md)|
|version|String|Version of the entity.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String"
}
```

