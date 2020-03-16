---
title: "workbookChartAxisFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartAxisFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartAxisFormat](../api/workbookchartaxisformat-get.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Read properties and relationships of the [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Update workbookChartAxisFormat](../api/workbookchartaxisformat-update.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Update the properties of a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Read properties and relationships of the [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|font|[workbookChartFont](../resources/workbookchartfont.md)||
|line|[workbookChartLineFormat](../resources/workbookchartlineformat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxisFormat",
  "id": "String (identifier)"
}
```

