---
title: "plannerTaskDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerTaskDetails resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Read properties and relationships of the [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[Update plannerTaskDetails](../api/plannertaskdetails-update.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Update the properties of a [plannerTaskDetails](../resources/plannertaskdetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checklist|[plannerChecklistItems](../resources/plannerchecklistitems.md)||
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|previewType|Enumeration|. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|references|[plannerExternalReferences](../resources/plannerexternalreferences.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerTaskDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "id": "String (identifier)",
  "description": "String",
  "previewType": "String",
  "references": {
    "@odata.type": "microsoft.graph.plannerExternalReferences"
  },
  "checklist": {
    "@odata.type": "microsoft.graph.plannerChecklistItems"
  }
}
```

