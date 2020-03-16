---
title: "workbookChartPointFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartPointFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartPointFormat](../api/workbookchartpointformat-get.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Read properties and relationships of the [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[Update workbookChartPointFormat](../api/workbookchartpointformat-update.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Update the properties of a [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read properties and relationships of the [workbookChartFill](../resources/workbookchartfill.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookchartfill.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartPointFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartPointFormat",
  "id": "String (identifier)"
}
```

