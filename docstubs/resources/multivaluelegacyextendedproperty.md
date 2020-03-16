---
title: "multiValueLegacyExtendedProperty resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# multiValueLegacyExtendedProperty resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get multiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty-get.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read properties and relationships of the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty-update.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
  "id": "String (identifier)",
  "value": [
    "String"
  ]
}
```

