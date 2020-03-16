---
title: "workbookTable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookTable resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookTable](../api/workbooktable-get.md)|[workbookTable](../resources/workbooktable.md)|Read properties and relationships of the [workbookTable](../resources/workbooktable.md) object.|
|[Update workbookTable](../api/workbooktable-update.md)|[workbookTable](../resources/workbooktable.md)|Update the properties of a [workbookTable](../resources/workbooktable.md) object.|
|[clearFilters](../api/workbooktable-clearfilters.md)|None||
|[convertToRange](../api/workbooktable-converttorange.md)|[workbookRange](../resources/workbookrange.md)||
|[dataBodyRange](../api/workbooktable-databodyrange.md)|[workbookRange](../resources/workbookrange.md)||
|[headerRowRange](../api/workbooktable-headerrowrange.md)|[workbookRange](../resources/workbookrange.md)||
|[range](../api/workbooktable-range.md)|[workbookRange](../resources/workbookrange.md)||
|[totalRowRange](../api/workbooktable-totalrowrange.md)|[workbookRange](../resources/workbookrange.md)||
|[reapplyFilters](../api/workbooktable-reapplyfilters.md)|None||
|[add](../api/workbooktable-add.md)|[workbookTable](../resources/workbooktable.md)||
|[itemAt](../api/workbooktable-itemat.md)|[workbookTable](../resources/workbooktable.md)||
|[count](../api/workbooktable-count.md)|Int32||
|[List columns](../api/workbooktable-list-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md) collection|Get the workbookTableColumns from the columns navigation property.|
|[Add columns](../api/workbooktable-post-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Add columns by posting to the columns collection.|
|[List rows](../api/workbooktable-list-rows.md)|[workbookTableRow](../resources/workbooktablerow.md) collection|Get the workbookTableRows from the rows navigation property.|
|[Add rows](../api/workbooktable-post-rows.md)|[workbookTableRow](../resources/workbooktablerow.md)|Add rows by posting to the rows collection.|
|[Get workbookTableSort](../api/workbooktablesort-get.md)|[workbookTableSort](../resources/workbooktablesort.md)|Read properties and relationships of the [workbookTableSort](../resources/workbooktablesort.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|highlightFirstColumn|Boolean||
|highlightLastColumn|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|legacyId|String||
|name|String||
|showBandedColumns|Boolean||
|showBandedRows|Boolean||
|showFilterButton|Boolean||
|showHeaders|Boolean||
|showTotals|Boolean||
|style|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|columns|[workbookTableColumn](../resources/workbooktablecolumn.md) collection||
|rows|[workbookTableRow](../resources/workbooktablerow.md) collection||
|sort|[workbookTableSort](../resources/workbooktablesort.md)||
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTable",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTable",
  "id": "String (identifier)",
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "legacyId": "String",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String"
}
```

