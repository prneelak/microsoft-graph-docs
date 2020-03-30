---
title: "taxGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# taxGroup resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get taxGroup](../api/taxgroup-get.md)|[taxGroup](../resources/taxgroup.md)|Read properties and relationships of the [taxGroup](../resources/taxgroup.md) object.|
|[Update taxGroup](../api/taxgroup-update.md)|[taxGroup](../resources/taxgroup.md)|Update the properties of a [taxGroup](../resources/taxgroup.md) object.|
|[List taxGroups](../api/company-list-taxgroups.md)|[taxGroup](../resources/taxgroup.md) collection|Get the taxGroups from the taxGroups navigation property.|
|[Add taxGroups](../api/company-post-taxgroups.md)|[taxGroup](../resources/taxgroup.md)|Add taxGroups by posting to the taxGroups collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|taxType|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taxGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taxGroup",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

