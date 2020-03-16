---
title: "mobileAppCategory resource type"
description: "Contains properties for a single Intune app category."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppCategory resource type


Namespace: microsoft.graph

Contains properties for a single Intune app category.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppCategory](../api/mobileappcategory-get.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Read properties and relationships of the [mobileAppCategory](../resources/mobileappcategory.md) object.|
|[Update mobileAppCategory](../api/mobileappcategory-update.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Update the properties of a [mobileAppCategory](../resources/mobileappcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the app category.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the mobileAppCategory was last modified.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

