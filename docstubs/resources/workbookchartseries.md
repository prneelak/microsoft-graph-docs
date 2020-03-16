---
title: "workbookChartSeries resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartSeries resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartSeries](../api/workbookchartseries-get.md)|[workbookChartSeries](../resources/workbookchartseries.md)|Read properties and relationships of the [workbookChartSeries](../resources/workbookchartseries.md) object.|
|[Update workbookChartSeries](../api/workbookchartseries-update.md)|[workbookChartSeries](../resources/workbookchartseries.md)|Update the properties of a [workbookChartSeries](../resources/workbookchartseries.md) object.|
|[itemAt](../api/workbookchartseries-itemat.md)|[workbookChartSeries](../resources/workbookchartseries.md)||
|[count](../api/workbookchartseries-count.md)|Int32||
|[Get workbookChartSeriesFormat](../api/workbookchartseriesformat-get.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|Read properties and relationships of the [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.|
|[List points](../api/workbookchartseries-list-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md) collection|Get the workbookChartPoints from the points navigation property.|
|[Add points](../api/workbookchartseries-post-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Add points by posting to the points collection.|
|[List series](../api/workbookchart-list-series.md)|[workbookChartSeries](../resources/workbookchartseries.md) collection|Get the workbookChartSerieses from the series navigation property.|
|[Add series](../api/workbookchart-post-series.md)|[workbookChartSeries](../resources/workbookchartseries.md)|Add series by posting to the series collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)||
|points|[workbookChartPoint](../resources/workbookchartpoint.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartSeries",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartSeries",
  "id": "String (identifier)",
  "name": "String"
}
```

