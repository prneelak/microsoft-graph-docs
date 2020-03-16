---
title: "workbookChartAxis resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartAxis resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Update workbookChartAxis](../api/workbookchartaxis-update.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Update the properties of a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Get workbookChartAxisFormat](../api/workbookchartaxisformat-get.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Read properties and relationships of the [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Get workbookChartGridlines](../api/workbookchartgridlines-get.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Read properties and relationships of the [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Get workbookChartGridlines](../api/workbookchartgridlines-get.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Read properties and relationships of the [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Get workbookChartAxisTitle](../api/workbookchartaxistitle-get.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Read properties and relationships of the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|majorUnit|[Json](../resources/json.md)||
|maximum|[Json](../resources/json.md)||
|minimum|[Json](../resources/json.md)||
|minorUnit|[Json](../resources/json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)||
|majorGridlines|[workbookChartGridlines](../resources/workbookchartgridlines.md)||
|minorGridlines|[workbookChartGridlines](../resources/workbookchartgridlines.md)||
|title|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxis",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxis",
  "id": "String (identifier)",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

