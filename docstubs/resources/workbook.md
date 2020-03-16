---
title: "workbook resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbook resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbook](../api/workbook-get.md)|[workbook](../resources/workbook.md)|Read properties and relationships of the [workbook](../resources/workbook.md) object.|
|[Update workbook](../api/workbook-update.md)|[workbook](../resources/workbook.md)|Update the properties of a [workbook](../resources/workbook.md) object.|
|[createSession](../api/workbook-createsession.md)|[workbookSessionInfo](../resources/workbooksessioninfo.md)||
|[closeSession](../api/workbook-closesession.md)|None||
|[refreshSession](../api/workbook-refreshsession.md)|None||
|[Get workbookApplication](../api/workbookapplication-get.md)|[workbookApplication](../resources/workbookapplication.md)|Read properties and relationships of the [workbookApplication](../resources/workbookapplication.md) object.|
|[List names](../api/workbook-list-names.md)|[workbookNamedItem](../resources/workbooknameditem.md) collection|Get the workbookNamedItems from the names navigation property.|
|[Add names](../api/workbook-post-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Add names by posting to the names collection.|
|[List tables](../api/workbook-list-tables.md)|[workbookTable](../resources/workbooktable.md) collection|Get the workbookTables from the tables navigation property.|
|[Add tables](../api/workbook-post-tables.md)|[workbookTable](../resources/workbooktable.md)|Add tables by posting to the tables collection.|
|[List worksheets](../api/workbook-list-worksheets.md)|[workbookWorksheet](../resources/workbookworksheet.md) collection|Get the workbookWorksheets from the worksheets navigation property.|
|[Add worksheets](../api/workbook-post-worksheets.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Add worksheets by posting to the worksheets collection.|
|[List comments](../api/workbook-list-comments.md)|[workbookComment](../resources/workbookcomment.md) collection|Get the workbookComments from the comments navigation property.|
|[Add comments](../api/workbook-post-comments.md)|[workbookComment](../resources/workbookcomment.md)|Add comments by posting to the comments collection.|
|[Get workbookFunctions](../api/workbookfunctions-get.md)|[workbookFunctions](../resources/workbookfunctions.md)|Read properties and relationships of the [workbookFunctions](../resources/workbookfunctions.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|application|[workbookApplication](../resources/workbookapplication.md)||
|comments|[workbookComment](../resources/workbookcomment.md) collection||
|functions|[workbookFunctions](../resources/workbookfunctions.md)||
|names|[workbookNamedItem](../resources/workbooknameditem.md) collection||
|tables|[workbookTable](../resources/workbooktable.md) collection||
|worksheets|[workbookWorksheet](../resources/workbookworksheet.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbook",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbook",
  "id": "String (identifier)"
}
```

