---
title: "schemaExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# schemaExtension resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List schemaExtensions](../api/schemaextension-list.md)|[schemaExtension](../resources/schemaextension.md) collection|List properties and relationships of the [schemaExtension](../resources/schemaextension.md) objects.|
|[Get schemaExtension](../api/schemaextension-get.md)|[schemaExtension](../resources/schemaextension.md)|Read properties and relationships of the [schemaExtension](../resources/schemaextension.md) object.|
|[Create schemaExtension](../api/schemaextension-post-schemaextensions.md)|[schemaExtension](../resources/schemaextension.md)|Create a new [schemaExtension](../resources/schemaextension.md) object.|
|[Delete schemaExtension](../api/schemaextension-delete.md)|None|Deletes a [schemaExtension](../resources/schemaextension.md).|
|[Update schemaExtension](../api/schemaextension-update.md)|[schemaExtension](../resources/schemaextension.md)|Update the properties of a [schemaExtension](../resources/schemaextension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|owner|String||
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection||
|status|String||
|targetTypes|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schemaExtension",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.schemaExtension",
  "id": "String (identifier)",
  "description": "String",
  "targetTypes": [
    "String"
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.extensionSchemaProperty"
    }
  ],
  "status": "String",
  "owner": "String"
}
```

