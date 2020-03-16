---
title: "workbookChartGridlines resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartGridlines resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartGridlines](../api/workbookchartgridlines-get.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Read properties and relationships of the [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Update workbookChartGridlines](../api/workbookchartgridlines-update.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Update the properties of a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Get workbookChartGridlinesFormat](../api/workbookchartgridlinesformat-get.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Read properties and relationships of the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|visible|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartGridlines",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartGridlines",
  "id": "String (identifier)",
  "visible": true
}
```

