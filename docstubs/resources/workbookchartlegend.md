---
title: "workbookChartLegend resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartLegend resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartLegend](../api/workbookchartlegend-get.md)|[workbookChartLegend](../resources/workbookchartlegend.md)|Read properties and relationships of the [workbookChartLegend](../resources/workbookchartlegend.md) object.|
|[Update workbookChartLegend](../api/workbookchartlegend-update.md)|[workbookChartLegend](../resources/workbookchartlegend.md)|Update the properties of a [workbookChartLegend](../resources/workbookchartlegend.md) object.|
|[Get workbookChartLegendFormat](../api/workbookchartlegendformat-get.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Read properties and relationships of the [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|overlay|Boolean||
|position|String||
|visible|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartLegend",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "id": "String (identifier)",
  "overlay": true,
  "position": "String",
  "visible": true
}
```

