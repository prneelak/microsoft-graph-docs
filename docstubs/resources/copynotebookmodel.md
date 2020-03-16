---
title: "CopyNotebookModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# CopyNotebookModel resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|String||
|createdByIdentity|[identitySet](../resources/identityset.md)||
|createdTime|DateTimeOffset||
|id|String||
|isDefault|Boolean||
|isShared|Boolean||
|lastModifiedBy|String||
|lastModifiedByIdentity|[identitySet](../resources/identityset.md)||
|lastModifiedTime|DateTimeOffset||
|links|[notebookLinks](../resources/notebooklinks.md)||
|name|String||
|sectionGroupsUrl|String||
|sectionsUrl|String||
|self|String||
|userRole|Enumeration|. Possible values are: `Owner`, `Contributor`, `Reader`, `None`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.CopyNotebookModel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.CopyNotebookModel",
  "isDefault": true,
  "userRole": "String",
  "isShared": true,
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "String"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "name": "String",
  "createdBy": "String",
  "createdByIdentity": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedBy": "String",
  "lastModifiedByIdentity": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedTime": "String (timestamp)",
  "id": "String (identifier)",
  "self": "String",
  "createdTime": "String (timestamp)"
}
```

