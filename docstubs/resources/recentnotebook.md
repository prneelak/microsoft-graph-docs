---
title: "recentNotebook resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# recentNotebook resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|lastAccessedTime|DateTimeOffset||
|links|[recentNotebookLinks](../resources/recentnotebooklinks.md)||
|sourceService|Enumeration|. Possible values are: `Unknown`, `OneDrive`, `OneDriveForBusiness`, `OnPremOneDriveForBusiness`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recentNotebook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recentNotebook",
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {
    "@odata.type": "microsoft.graph.recentNotebookLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "String"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  },
  "sourceService": "String"
}
```

