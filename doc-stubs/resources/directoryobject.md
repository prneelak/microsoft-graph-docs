---
title: "directoryObject resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# directoryObject resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List directoryObjects](../api/directoryobject-list.md)|[directoryObject](../resources/directoryobject.md) collection|Get a list of the [directoryObject](../resources/directoryobject.md) objects and their properties.|
|[Create directoryObject](../api/directoryobject-post-directoryobjects.md)|[directoryObject](../resources/directoryobject.md)|Create a new [directoryObject](../resources/directoryobject.md) object.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read the properties and relationships of a [directoryObject](../resources/directoryobject.md) object.|
|[Update directoryObject](../api/directoryobject-update.md)|[directoryObject](../resources/directoryobject.md)|Update the properties of a [directoryObject](../resources/directoryobject.md) object.|
|[Delete directoryObject](../api/directoryobject-delete.md)|None|Deletes a [directoryObject](../resources/directoryobject.md) object.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Boolean collection|**TODO: Add Description**|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "String (identifier)",
  "deletedDateTime": "String"
}
```

