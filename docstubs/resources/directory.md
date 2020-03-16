---
title: "directory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# directory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get directory](../api/directory-get.md)|[directory](../resources/directory.md)|Read properties and relationships of the [directory](../resources/directory.md) object.|
|[Update directory](../api/directory-update.md)|[directory](../resources/directory.md)|Update the properties of a [directory](../resources/directory.md) object.|
|[List deletedItems](../api/directory-list-deleteditems.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the deletedItems navigation property.|
|[Add deletedItems](../api/directory-post-deleteditems.md)|[directoryObject](../resources/directoryobject.md)|Add deletedItems by posting to the deletedItems collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deletedItems|[directoryObject](../resources/directoryobject.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directory",
  "id": "String (identifier)"
}
```

