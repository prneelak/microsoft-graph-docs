---
title: "columnLink resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# columnLink resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get columnLink](../api/columnlink-get.md)|[columnLink](../resources/columnlink.md)|Read properties and relationships of the [columnLink](../resources/columnlink.md) object.|
|[Update columnLink](../api/columnlink-update.md)|[columnLink](../resources/columnlink.md)|Update the properties of a [columnLink](../resources/columnlink.md) object.|
|[List columnLinks](../api/contenttype-list-columnlinks.md)|[columnLink](../resources/columnlink.md) collection|Get the columnLinks from the columnLinks navigation property.|
|[Add columnLinks](../api/contenttype-post-columnlinks.md)|[columnLink](../resources/columnlink.md)|Add columnLinks by posting to the columnLinks collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.columnLink",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.columnLink",
  "id": "String (identifier)",
  "name": "String"
}
```

