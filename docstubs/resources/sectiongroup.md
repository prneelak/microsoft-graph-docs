---
title: "sectionGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sectionGroup resource type


Namespace: microsoft.graph




Inherits from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectiongroup.md)|Read properties and relationships of the [sectionGroup](../resources/sectiongroup.md) object.|
|[Update sectionGroup](../api/sectiongroup-update.md)|[sectionGroup](../resources/sectiongroup.md)|Update the properties of a [sectionGroup](../resources/sectiongroup.md) object.|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read properties and relationships of the [notebook](../resources/notebook.md) object.|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectiongroup.md)|Read properties and relationships of the [sectionGroup](../resources/sectiongroup.md) object.|
|[List sections](../api/sectiongroup-list-sections.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Add sections](../api/sectiongroup-post-sections.md)|[onenoteSection](../resources/onenotesection.md)|Add sections by posting to the sections collection.|
|[List sectionGroups](../api/sectiongroup-list-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the sectionGroups navigation property.|
|[Add sectionGroups](../api/sectiongroup-post-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Add sectionGroups by posting to the sectionGroups collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|sectionGroupsUrl|String||
|sectionsUrl|String||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|parentNotebook|[notebook](../resources/notebook.md)||
|parentSectionGroup|[sectionGroup](../resources/sectiongroup.md)||
|sectionGroups|[sectionGroup](../resources/sectiongroup.md) collection||
|sections|[onenoteSection](../resources/onenotesection.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sectionGroup",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sectionGroup",
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
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String"
}
```

