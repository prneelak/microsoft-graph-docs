---
title: "onenoteResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenoteResource resource type


Namespace: microsoft.graph




Inherits from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenoteResource](../api/onenoteresource-get.md)|[onenoteResource](../resources/onenoteresource.md)|Read properties and relationships of the [onenoteResource](../resources/onenoteresource.md) object.|
|[Update onenoteResource](../api/onenoteresource-update.md)|[onenoteResource](../resources/onenoteresource.md)|Update the properties of a [onenoteResource](../resources/onenoteresource.md) object.|
|[List resources](../api/onenote-list-resources.md)|[onenoteResource](../resources/onenoteresource.md) collection|Get the onenoteResources from the resources navigation property.|
|[Add resources](../api/onenote-post-resources.md)|[onenoteResource](../resources/onenoteresource.md)|Add resources by posting to the resources collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream||
|contentUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteResource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "id": "String (identifier)",
  "self": "String",
  "content": "Stream",
  "contentUrl": "String"
}
```

