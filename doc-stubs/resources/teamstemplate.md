---
title: "teamsTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teamsTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List teamsTemplates](../api/teamstemplate-list.md)|[teamsTemplate](../resources/teamstemplate.md) collection|Get a list of the [teamsTemplate](../resources/teamstemplate.md) objects and their properties.|
|[Get teamsTemplate](../api/teamstemplate-get.md)|[teamsTemplate](../resources/teamstemplate.md)|Read the properties and relationships of a [teamsTemplate](../resources/teamstemplate.md) object.|
|[Create teamsTemplate](../api/teamstemplate-post-teamstemplates.md)|[teamsTemplate](../resources/teamstemplate.md)|Create a new [teamsTemplate](../resources/teamstemplate.md) object.|
|[Delete teamsTemplate](../api/teamstemplate-delete.md)|None|Deletes a [teamsTemplate](../resources/teamstemplate.md) object.|
|[Update teamsTemplate](../api/teamstemplate-update.md)|[teamsTemplate](../resources/teamstemplate.md)|Update the properties of a [teamsTemplate](../resources/teamstemplate.md) object.|
|[List template](../api/team-list-template.md)|[teamsTemplate](../resources/teamstemplate.md) collection|Get the teamsTemplates from the template navigation property.|
|[Add template](../api/team-post-template.md)|[teamsTemplate](../resources/teamstemplate.md)|Add template by posting to the template collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsTemplate",
  "id": "String (identifier)"
}
```

