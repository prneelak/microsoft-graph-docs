---
title: "workbookChartLineFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartLineFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartLineFormats](../api/workbookchartlineformat-list.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md) collection|List properties and relationships of the [workbookChartLineFormat](../resources/workbookchartlineformat.md) objects.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Read properties and relationships of the [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[Create workbookChartLineFormat](../api/workbookchartlineformat-create.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Create a new [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[Delete workbookChartLineFormat](../api/workbookchartlineformat-delete.md)|None|Deletes a [workbookChartLineFormat](../resources/workbookchartlineformat.md).|
|[Update workbookChartLineFormat](../api/workbookchartlineformat-update.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Update the properties of a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[clear](../api/workbookchartlineformat-clear.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartLineFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartLineFormat",
  "id": "String (identifier)",
  "color": "String"
}
```

