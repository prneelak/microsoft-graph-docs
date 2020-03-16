---
title: "workbookWorksheet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookWorksheet resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[Update workbookWorksheet](../api/workbookworksheet-update.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Update the properties of a [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[cell](../api/workbookworksheet-cell.md)|[workbookRange](../resources/workbookrange.md)||
|[range](../api/workbookworksheet-range.md)|[workbookRange](../resources/workbookrange.md)||
|[range](../api/workbookworksheet-range.md)|[workbookRange](../resources/workbookrange.md)||
|[usedRange](../api/workbookworksheet-usedrange.md)|[workbookRange](../resources/workbookrange.md)||
|[usedRange](../api/workbookworksheet-usedrange.md)|[workbookRange](../resources/workbookrange.md)||
|[add](../api/workbookworksheet-add.md)|[workbookWorksheet](../resources/workbookworksheet.md)||
|[List charts](../api/workbookworksheet-list-charts.md)|[workbookChart](../resources/workbookchart.md) collection|Get the workbookCharts from the charts navigation property.|
|[Add charts](../api/workbookworksheet-post-charts.md)|[workbookChart](../resources/workbookchart.md)|Add charts by posting to the charts collection.|
|[List names](../api/workbookworksheet-list-names.md)|[workbookNamedItem](../resources/workbooknameditem.md) collection|Get the workbookNamedItems from the names navigation property.|
|[Add names](../api/workbookworksheet-post-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Add names by posting to the names collection.|
|[List pivotTables](../api/workbookworksheet-list-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md) collection|Get the workbookPivotTables from the pivotTables navigation property.|
|[Add pivotTables](../api/workbookworksheet-post-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Add pivotTables by posting to the pivotTables collection.|
|[Get workbookWorksheetProtection](../api/workbookworksheetprotection-get.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Read properties and relationships of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[List tables](../api/workbookworksheet-list-tables.md)|[workbookTable](../resources/workbooktable.md) collection|Get the workbookTables from the tables navigation property.|
|[Add tables](../api/workbookworksheet-post-tables.md)|[workbookTable](../resources/workbooktable.md)|Add tables by posting to the tables collection.|
|[List worksheets](../api/workbook-list-worksheets.md)|[workbookWorksheet](../resources/workbookworksheet.md) collection|Get the workbookWorksheets from the worksheets navigation property.|
|[Add worksheets](../api/workbook-post-worksheets.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Add worksheets by posting to the worksheets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|position|Int32||
|visibility|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|charts|[workbookChart](../resources/workbookchart.md) collection||
|names|[workbookNamedItem](../resources/workbooknameditem.md) collection||
|pivotTables|[workbookPivotTable](../resources/workbookpivottable.md) collection||
|protection|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)||
|tables|[workbookTable](../resources/workbooktable.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "id": "String (identifier)",
  "name": "String",
  "position": 1024,
  "visibility": "String"
}
```

