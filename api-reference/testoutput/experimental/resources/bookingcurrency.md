---
title: "bookingCurrency resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingCurrency resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List bookingCurrencies](../api/bookingcurrency-list.md)|[bookingCurrency](../resources/bookingcurrency.md) collection|List properties and relationships of the [bookingCurrency](../resources/bookingcurrency.md) objects.|
|[Get bookingCurrency](../api/bookingcurrency-get.md)|[bookingCurrency](../resources/bookingcurrency.md)|Read properties and relationships of the [bookingCurrency](../resources/bookingcurrency.md) object.|
|[Create bookingCurrency](../api/bookingcurrency-post-bookingcurrencies.md)|[bookingCurrency](../resources/bookingcurrency.md)|Create a new [bookingCurrency](../resources/bookingcurrency.md) object.|
|[Delete bookingCurrency](../api/bookingcurrency-delete.md)|None|Deletes a [bookingCurrency](../resources/bookingcurrency.md).|
|[Update bookingCurrency](../api/bookingcurrency-update.md)|[bookingCurrency](../resources/bookingcurrency.md)|Update the properties of a [bookingCurrency](../resources/bookingcurrency.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|symbol|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCurrency",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "id": "String (identifier)",
  "symbol": "String"
}
```

