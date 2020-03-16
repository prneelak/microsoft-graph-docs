---
title: "workbookTableColumn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookTableColumn resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookTableColumn](../api/workbooktablecolumn-get.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Read properties and relationships of the [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[Update workbookTableColumn](../api/workbooktablecolumn-update.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Update the properties of a [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[dataBodyRange](../api/workbooktablecolumn-databodyrange.md)|[workbookRange](../resources/workbookrange.md)||
|[headerRowRange](../api/workbooktablecolumn-headerrowrange.md)|[workbookRange](../resources/workbookrange.md)||
|[range](../api/workbooktablecolumn-range.md)|[workbookRange](../resources/workbookrange.md)||
|[totalRowRange](../api/workbooktablecolumn-totalrowrange.md)|[workbookRange](../resources/workbookrange.md)||
|[add](../api/workbooktablecolumn-add.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)||
|[itemAt](../api/workbooktablecolumn-itemat.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)||
|[count](../api/workbooktablecolumn-count.md)|Int32||
|[Get workbookFilter](../api/workbookfilter-get.md)|[workbookFilter](../resources/workbookfilter.md)|Read properties and relationships of the [workbookFilter](../resources/workbookfilter.md) object.|
|[List columns](../api/workbooktable-list-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md) collection|Get the workbookTableColumns from the columns navigation property.|
|[Add columns](../api/workbooktable-post-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Add columns by posting to the columns collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|name|String||
|values|[Json](../resources/json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|filter|[workbookFilter](../resources/workbookfilter.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableColumn",
  "id": "String (identifier)",
  "index": 1024,
  "name": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

