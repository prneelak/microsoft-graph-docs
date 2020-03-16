---
title: "workbookChartAreaFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartAreaFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartAreaFormat](../api/workbookchartareaformat-get.md)|[workbookChartAreaFormat](../resources/workbookchartareaformat.md)|Read properties and relationships of the [workbookChartAreaFormat](../resources/workbookchartareaformat.md) object.|
|[Update workbookChartAreaFormat](../api/workbookchartareaformat-update.md)|[workbookChartAreaFormat](../resources/workbookchartareaformat.md)|Update the properties of a [workbookChartAreaFormat](../resources/workbookchartareaformat.md) object.|
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
  "@odata.type": "microsoft.graph.workbookChartAreaFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAreaFormat",
  "id": "String (identifier)"
}
```

