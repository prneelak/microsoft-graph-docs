---
title: "columnDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# columnDefinition resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get columnDefinition](../api/columndefinition-get.md)|[columnDefinition](../resources/columndefinition.md)|Read properties and relationships of the [columnDefinition](../resources/columndefinition.md) object.|
|[Update columnDefinition](../api/columndefinition-update.md)|[columnDefinition](../resources/columndefinition.md)|Update the properties of a [columnDefinition](../resources/columndefinition.md) object.|
|[List columns](../api/site-list-columns.md)|[columnDefinition](../resources/columndefinition.md) collection|Get the columnDefinitions from the columns navigation property.|
|[Add columns](../api/site-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Add columns by posting to the columns collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|boolean|[booleanColumn](../resources/booleancolumn.md)||
|calculated|[calculatedColumn](../resources/calculatedcolumn.md)||
|choice|[choiceColumn](../resources/choicecolumn.md)||
|columnGroup|String||
|currency|[currencyColumn](../resources/currencycolumn.md)||
|dateTime|[dateTimeColumn](../resources/datetimecolumn.md)||
|defaultValue|[defaultColumnValue](../resources/defaultcolumnvalue.md)||
|description|String||
|displayName|String||
|enforceUniqueValues|Boolean||
|hidden|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|indexed|Boolean||
|lookup|[lookupColumn](../resources/lookupcolumn.md)||
|name|String||
|number|[numberColumn](../resources/numbercolumn.md)||
|personOrGroup|[personOrGroupColumn](../resources/personorgroupcolumn.md)||
|readOnly|Boolean||
|required|Boolean||
|text|[textColumn](../resources/textcolumn.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.columnDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.columnDefinition",
  "id": "String (identifier)",
  "boolean": {
    "@odata.type": "microsoft.graph.booleanColumn"
  },
  "calculated": {
    "@odata.type": "microsoft.graph.calculatedColumn"
  },
  "choice": {
    "@odata.type": "microsoft.graph.choiceColumn"
  },
  "columnGroup": "String",
  "currency": {
    "@odata.type": "microsoft.graph.currencyColumn"
  },
  "dateTime": {
    "@odata.type": "microsoft.graph.dateTimeColumn"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.defaultColumnValue"
  },
  "description": "String",
  "displayName": "String",
  "enforceUniqueValues": true,
  "hidden": true,
  "indexed": true,
  "lookup": {
    "@odata.type": "microsoft.graph.lookupColumn"
  },
  "name": "String",
  "number": {
    "@odata.type": "microsoft.graph.numberColumn"
  },
  "personOrGroup": {
    "@odata.type": "microsoft.graph.personOrGroupColumn"
  },
  "readOnly": true,
  "required": true,
  "text": {
    "@odata.type": "microsoft.graph.textColumn"
  }
}
```

