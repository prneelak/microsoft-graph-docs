---
title: "workbookPivotTable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookPivotTable resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookPivotTable](../api/workbookpivottable-get.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Read properties and relationships of the [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Update workbookPivotTable](../api/workbookpivottable-update.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Update the properties of a [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[refresh](../api/workbookpivottable-refresh.md)|None||
|[refreshAll](../api/workbookpivottable-refreshall.md)|None||
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[List pivotTables](../api/workbookworksheet-list-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md) collection|Get the workbookPivotTables from the pivotTables navigation property.|
|[Add pivotTables](../api/workbookworksheet-post-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Add pivotTables by posting to the pivotTables collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookPivotTable",
  "id": "String (identifier)",
  "name": "String"
}
```

