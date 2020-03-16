---
title: "notebook resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# notebook resource type


Namespace: microsoft.graph




Inherits from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read properties and relationships of the [notebook](../resources/notebook.md) object.|
|[Update notebook](../api/notebook-update.md)|[notebook](../resources/notebook.md)|Update the properties of a [notebook](../resources/notebook.md) object.|
|[copyNotebook](../api/notebook-copynotebook.md)|[onenoteOperation](../resources/onenoteoperation.md)||
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md)|[recentNotebook](../resources/recentnotebook.md) collection||
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md)|[CopyNotebookModel](../resources/copynotebookmodel.md)||
|[List sections](../api/notebook-list-sections.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Add sections](../api/notebook-post-sections.md)|[onenoteSection](../resources/onenotesection.md)|Add sections by posting to the sections collection.|
|[List sectionGroups](../api/notebook-list-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the sectionGroups navigation property.|
|[Add sectionGroups](../api/notebook-post-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Add sectionGroups by posting to the sectionGroups collection.|
|[List notebooks](../api/onenote-list-notebooks.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the notebooks navigation property.|
|[Add notebooks](../api/onenote-post-notebooks.md)|[notebook](../resources/notebook.md)|Add notebooks by posting to the notebooks collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|isShared|Boolean||
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|links|[notebookLinks](../resources/notebooklinks.md)||
|sectionGroupsUrl|String||
|sectionsUrl|String||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|userRole|Enumeration|. Possible values are: `Owner`, `Contributor`, `Reader`, `None`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sectionGroups|[sectionGroup](../resources/sectiongroup.md) collection||
|sections|[onenoteSection](../resources/onenotesection.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notebook",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notebook",
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
  "userRole": "String",
  "isShared": true,
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks"
  }
}
```

