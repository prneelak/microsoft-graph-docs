---
title: "workbookTableRow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookTableRow resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookTableRow](../api/workbooktablerow-get.md)|[workbookTableRow](../resources/workbooktablerow.md)|Read properties and relationships of the [workbookTableRow](../resources/workbooktablerow.md) object.|
|[Update workbookTableRow](../api/workbooktablerow-update.md)|[workbookTableRow](../resources/workbooktablerow.md)|Update the properties of a [workbookTableRow](../resources/workbooktablerow.md) object.|
|[range](../api/workbooktablerow-range.md)|[workbookRange](../resources/workbookrange.md)||
|[add](../api/workbooktablerow-add.md)|[workbookTableRow](../resources/workbooktablerow.md)||
|[itemAt](../api/workbooktablerow-itemat.md)|[workbookTableRow](../resources/workbooktablerow.md)||
|[count](../api/workbooktablerow-count.md)|Int32||
|[List rows](../api/workbooktable-list-rows.md)|[workbookTableRow](../resources/workbooktablerow.md) collection|Get the workbookTableRows from the rows navigation property.|
|[Add rows](../api/workbooktable-post-rows.md)|[workbookTableRow](../resources/workbooktablerow.md)|Add rows by posting to the rows collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|values|[Json](../resources/json.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTableRow",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "id": "String (identifier)",
  "index": 1024,
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

