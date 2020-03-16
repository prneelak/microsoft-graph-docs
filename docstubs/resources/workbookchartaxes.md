---
title: "workbookChartAxes resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartAxes resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartAxes](../api/workbookchartaxes-get.md)|[workbookChartAxes](../resources/workbookchartaxes.md)|Read properties and relationships of the [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Update workbookChartAxes](../api/workbookchartaxes-update.md)|[workbookChartAxes](../resources/workbookchartaxes.md)|Update the properties of a [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categoryAxis|[workbookChartAxis](../resources/workbookchartaxis.md)||
|seriesAxis|[workbookChartAxis](../resources/workbookchartaxis.md)||
|valueAxis|[workbookChartAxis](../resources/workbookchartaxis.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxes",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxes",
  "id": "String (identifier)"
}
```

