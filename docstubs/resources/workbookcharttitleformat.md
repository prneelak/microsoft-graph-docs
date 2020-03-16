---
title: "workbookChartTitleFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartTitleFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartTitleFormat](../api/workbookcharttitleformat-get.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Read properties and relationships of the [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Update workbookChartTitleFormat](../api/workbookcharttitleformat-update.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Update the properties of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read properties and relationships of the [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookchartfill.md)||
|font|[workbookChartFont](../resources/workbookchartfont.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartTitleFormat",
  "id": "String (identifier)"
}
```

