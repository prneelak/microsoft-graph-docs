---
title: "directoryObject resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# directoryObject resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryObjects](../api/directoryobject-list.md)|[directoryObject](../resources/directoryobject.md) collection|List properties and relationships of the [directoryObject](../resources/directoryobject.md) objects.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[Create directoryObject](../api/directoryobject-post-directoryobjects.md)|[directoryObject](../resources/directoryobject.md)|Create a new [directoryObject](../resources/directoryobject.md) object.|
|[Delete directoryObject](../api/directoryobject-delete.md)|None|Deletes a [directoryObject](../resources/directoryobject.md).|
|[Update directoryObject](../api/directoryobject-update.md)|[directoryObject](../resources/directoryobject.md)|Update the properties of a [directoryObject](../resources/directoryobject.md) object.|
|[getByIds](../api/directoryobject-getbyids.md)|[directoryObject](../resources/directoryobject.md) collection||
|[validateProperties](../api/directoryobject-validateproperties.md)|None||
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String collection||
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection||
|[restore](../api/directoryobject-restore.md)|[directoryObject](../resources/directoryobject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "deletedDateTime": "String (timestamp)"
}
```

