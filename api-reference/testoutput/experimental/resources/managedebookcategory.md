---
title: "managedEBookCategory resource type"
description: "Contains properties for a single Intune eBook category."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedEBookCategory resource type


Namespace: microsoft.graph

Contains properties for a single Intune eBook category.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBookCategory](../api/managedebookcategory-get.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Read properties and relationships of the [managedEBookCategory](../resources/managedebookcategory.md) object.|
|[Update managedEBookCategory](../api/managedebookcategory-update.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Update the properties of a [managedEBookCategory](../resources/managedebookcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the eBook category.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the ManagedEBookCategory was last modified.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

