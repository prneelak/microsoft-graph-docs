---
title: "workbookChartTitle resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartTitle resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartTitle](../api/workbookcharttitle-get.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Read properties and relationships of the [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Update workbookChartTitle](../api/workbookcharttitle-update.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Update the properties of a [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Get workbookChartTitleFormat](../api/workbookcharttitleformat-get.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Read properties and relationships of the [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|overlay|Boolean||
|text|String||
|visible|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartTitle",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "id": "String (identifier)",
  "overlay": true,
  "text": "String",
  "visible": true
}
```

