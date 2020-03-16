---
title: "workbookChart resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChart resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChart](../api/workbookchart-get.md)|[workbookChart](../resources/workbookchart.md)|Read properties and relationships of the [workbookChart](../resources/workbookchart.md) object.|
|[Update workbookChart](../api/workbookchart-update.md)|[workbookChart](../resources/workbookchart.md)|Update the properties of a [workbookChart](../resources/workbookchart.md) object.|
|[image](../api/workbookchart-image.md)|String||
|[image](../api/workbookchart-image.md)|String||
|[image](../api/workbookchart-image.md)|String||
|[image](../api/workbookchart-image.md)|String||
|[setData](../api/workbookchart-setdata.md)|None||
|[setPosition](../api/workbookchart-setposition.md)|None||
|[add](../api/workbookchart-add.md)|[workbookChart](../resources/workbookchart.md)||
|[item](../api/workbookchart-item.md)|[workbookChart](../resources/workbookchart.md)||
|[itemAt](../api/workbookchart-itemat.md)|[workbookChart](../resources/workbookchart.md)||
|[count](../api/workbookchart-count.md)|Int32||
|[Get workbookChartAxes](../api/workbookchartaxes-get.md)|[workbookChartAxes](../resources/workbookchartaxes.md)|Read properties and relationships of the [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Get workbookChartDataLabels](../api/workbookchartdatalabels-get.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Read properties and relationships of the [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[Get workbookChartAreaFormat](../api/workbookchartareaformat-get.md)|[workbookChartAreaFormat](../resources/workbookchartareaformat.md)|Read properties and relationships of the [workbookChartAreaFormat](../resources/workbookchartareaformat.md) object.|
|[Get workbookChartLegend](../api/workbookchartlegend-get.md)|[workbookChartLegend](../resources/workbookchartlegend.md)|Read properties and relationships of the [workbookChartLegend](../resources/workbookchartlegend.md) object.|
|[List series](../api/workbookchart-list-series.md)|[workbookChartSeries](../resources/workbookchartseries.md) collection|Get the workbookChartSerieses from the series navigation property.|
|[Add series](../api/workbookchart-post-series.md)|[workbookChartSeries](../resources/workbookchartseries.md)|Add series by posting to the series collection.|
|[Get workbookChartTitle](../api/workbookcharttitle-get.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Read properties and relationships of the [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[List charts](../api/workbookworksheet-list-charts.md)|[workbookChart](../resources/workbookchart.md) collection|Get the workbookCharts from the charts navigation property.|
|[Add charts](../api/workbookworksheet-post-charts.md)|[workbookChart](../resources/workbookchart.md)|Add charts by posting to the charts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|height|Double||
|id|String| Inherited from [entity](../resources/entity.md)|
|left|Double||
|name|String||
|top|Double||
|width|Double||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|axes|[workbookChartAxes](../resources/workbookchartaxes.md)||
|dataLabels|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)||
|format|[workbookChartAreaFormat](../resources/workbookchartareaformat.md)||
|legend|[workbookChartLegend](../resources/workbookchartlegend.md)||
|series|[workbookChartSeries](../resources/workbookchartseries.md) collection||
|title|[workbookChartTitle](../resources/workbookcharttitle.md)||
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChart",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChart",
  "id": "String (identifier)",
  "height": "Double",
  "left": "Double",
  "name": "String",
  "top": "Double",
  "width": "Double"
}
```

