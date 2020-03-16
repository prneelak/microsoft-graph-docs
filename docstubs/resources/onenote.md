---
title: "onenote resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenote resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read properties and relationships of the [onenote](../resources/onenote.md) object.|
|[Update onenote](../api/onenote-update.md)|[onenote](../resources/onenote.md)|Update the properties of a [onenote](../resources/onenote.md) object.|
|[List notebooks](../api/onenote-list-notebooks.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the notebooks navigation property.|
|[Add notebooks](../api/onenote-post-notebooks.md)|[notebook](../resources/notebook.md)|Add notebooks by posting to the notebooks collection.|
|[List sections](../api/onenote-list-sections.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Add sections](../api/onenote-post-sections.md)|[onenoteSection](../resources/onenotesection.md)|Add sections by posting to the sections collection.|
|[List sectionGroups](../api/onenote-list-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the sectionGroups navigation property.|
|[Add sectionGroups](../api/onenote-post-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Add sectionGroups by posting to the sectionGroups collection.|
|[List pages](../api/onenote-list-pages.md)|[onenotePage](../resources/onenotepage.md) collection|Get the onenotePages from the pages navigation property.|
|[Add pages](../api/onenote-post-pages.md)|[onenotePage](../resources/onenotepage.md)|Add pages by posting to the pages collection.|
|[List resources](../api/onenote-list-resources.md)|[onenoteResource](../resources/onenoteresource.md) collection|Get the onenoteResources from the resources navigation property.|
|[Add resources](../api/onenote-post-resources.md)|[onenoteResource](../resources/onenoteresource.md)|Add resources by posting to the resources collection.|
|[List operations](../api/onenote-list-operations.md)|[onenoteOperation](../resources/onenoteoperation.md) collection|Get the onenoteOperations from the operations navigation property.|
|[Add operations](../api/onenote-post-operations.md)|[onenoteOperation](../resources/onenoteoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|notebooks|[notebook](../resources/notebook.md) collection||
|operations|[onenoteOperation](../resources/onenoteoperation.md) collection||
|pages|[onenotePage](../resources/onenotepage.md) collection||
|resources|[onenoteResource](../resources/onenoteresource.md) collection||
|sectionGroups|[sectionGroup](../resources/sectiongroup.md) collection||
|sections|[onenoteSection](../resources/onenotesection.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenote",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenote",
  "id": "String (identifier)"
}
```

