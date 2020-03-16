---
title: "workbookFilter resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookFilter resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookFilter](../api/workbookfilter-get.md)|[workbookFilter](../resources/workbookfilter.md)|Read properties and relationships of the [workbookFilter](../resources/workbookfilter.md) object.|
|[Update workbookFilter](../api/workbookfilter-update.md)|[workbookFilter](../resources/workbookfilter.md)|Update the properties of a [workbookFilter](../resources/workbookfilter.md) object.|
|[apply](../api/workbookfilter-apply.md)|None||
|[applyBottomItemsFilter](../api/workbookfilter-applybottomitemsfilter.md)|None||
|[applyBottomPercentFilter](../api/workbookfilter-applybottompercentfilter.md)|None||
|[applyCellColorFilter](../api/workbookfilter-applycellcolorfilter.md)|None||
|[applyCustomFilter](../api/workbookfilter-applycustomfilter.md)|None||
|[applyDynamicFilter](../api/workbookfilter-applydynamicfilter.md)|None||
|[applyFontColorFilter](../api/workbookfilter-applyfontcolorfilter.md)|None||
|[applyIconFilter](../api/workbookfilter-applyiconfilter.md)|None||
|[applyTopItemsFilter](../api/workbookfilter-applytopitemsfilter.md)|None||
|[applyTopPercentFilter](../api/workbookfilter-applytoppercentfilter.md)|None||
|[applyValuesFilter](../api/workbookfilter-applyvaluesfilter.md)|None||
|[clear](../api/workbookfilter-clear.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|criteria|[workbookFilterCriteria](../resources/workbookfiltercriteria.md)||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookFilter",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "id": "String (identifier)",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria"
  }
}
```

