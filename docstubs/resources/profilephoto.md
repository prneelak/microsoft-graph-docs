---
title: "profilePhoto resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# profilePhoto resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get profilePhoto](../api/profilephoto-get.md)|[profilePhoto](../resources/profilephoto.md)|Read properties and relationships of the [profilePhoto](../resources/profilephoto.md) object.|
|[Update profilePhoto](../api/profilephoto-update.md)|[profilePhoto](../resources/profilephoto.md)|Update the properties of a [profilePhoto](../resources/profilephoto.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|height|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|width|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "id": "String (identifier)",
  "height": 1024,
  "width": 1024
}
```

