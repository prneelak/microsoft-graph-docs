---
title: "workbookChartPoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartPoint resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartPoint](../api/workbookchartpoint-get.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Read properties and relationships of the [workbookChartPoint](../resources/workbookchartpoint.md) object.|
|[Update workbookChartPoint](../api/workbookchartpoint-update.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Update the properties of a [workbookChartPoint](../resources/workbookchartpoint.md) object.|
|[itemAt](../api/workbookchartpoint-itemat.md)|[workbookChartPoint](../resources/workbookchartpoint.md)||
|[count](../api/workbookchartpoint-count.md)|Int32||
|[Get workbookChartPointFormat](../api/workbookchartpointformat-get.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Read properties and relationships of the [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[List points](../api/workbookchartseries-list-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md) collection|Get the workbookChartPoints from the points navigation property.|
|[Add points](../api/workbookchartseries-post-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Add points by posting to the points collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|[Json](../resources/json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartPointFormat](../resources/workbookchartpointformat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartPoint",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartPoint",
  "id": "String (identifier)",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

