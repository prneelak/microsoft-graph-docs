---
title: "workbookNamedItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookNamedItem resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookNamedItem](../api/workbooknameditem-get.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Read properties and relationships of the [workbookNamedItem](../resources/workbooknameditem.md) object.|
|[Update workbookNamedItem](../api/workbooknameditem-update.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Update the properties of a [workbookNamedItem](../resources/workbooknameditem.md) object.|
|[range](../api/workbooknameditem-range.md)|[workbookRange](../resources/workbookrange.md)||
|[add](../api/workbooknameditem-add.md)|[workbookNamedItem](../resources/workbooknameditem.md)||
|[addFormulaLocal](../api/workbooknameditem-addformulalocal.md)|[workbookNamedItem](../resources/workbooknameditem.md)||
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[List names](../api/workbook-list-names.md)|[workbookNamedItem](../resources/workbooknameditem.md) collection|Get the workbookNamedItems from the names navigation property.|
|[Add names](../api/workbook-post-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Add names by posting to the names collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|comment|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|scope|String||
|type|String||
|value|[Json](../resources/json.md)||
|visible|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "id": "String (identifier)",
  "comment": "String",
  "name": "String",
  "scope": "String",
  "type": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": true
}
```

