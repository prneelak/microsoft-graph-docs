---
title: "workbookChartSeriesFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartSeriesFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartSeriesFormat](../api/workbookchartseriesformat-get.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|Read properties and relationships of the [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.|
|[Update workbookChartSeriesFormat](../api/workbookchartseriesformat-update.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|Update the properties of a [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read properties and relationships of the [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Read properties and relationships of the [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookchartfill.md)||
|line|[workbookChartLineFormat](../resources/workbookchartlineformat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartSeriesFormat",
  "id": "String (identifier)"
}
```

