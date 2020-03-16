---
title: "onenoteSection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenoteSection resource type


Namespace: microsoft.graph




Inherits from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenotesection.md)|Read properties and relationships of the [onenoteSection](../resources/onenotesection.md) object.|
|[Update onenoteSection](../api/onenotesection-update.md)|[onenoteSection](../resources/onenotesection.md)|Update the properties of a [onenoteSection](../resources/onenotesection.md) object.|
|[copyToNotebook](../api/onenotesection-copytonotebook.md)|[onenoteOperation](../resources/onenoteoperation.md)||
|[copyToSectionGroup](../api/onenotesection-copytosectiongroup.md)|[onenoteOperation](../resources/onenoteoperation.md)||
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read properties and relationships of the [notebook](../resources/notebook.md) object.|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectiongroup.md)|Read properties and relationships of the [sectionGroup](../resources/sectiongroup.md) object.|
|[List pages](../api/onenotesection-list-pages.md)|[onenotePage](../resources/onenotepage.md) collection|Get the onenotePages from the pages navigation property.|
|[Add pages](../api/onenotesection-post-pages.md)|[onenotePage](../resources/onenotepage.md)|Add pages by posting to the pages collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|links|[sectionLinks](../resources/sectionlinks.md)||
|pagesUrl|String||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|pages|[onenotePage](../resources/onenotepage.md) collection||
|parentNotebook|[notebook](../resources/notebook.md)||
|parentSectionGroup|[sectionGroup](../resources/sectiongroup.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteSection",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteSection",
  "id": "String (identifier)",
  "self": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isDefault": true,
  "links": {
    "@odata.type": "microsoft.graph.sectionLinks"
  },
  "pagesUrl": "String"
}
```

