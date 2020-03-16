---
title: "iosHomeScreenFolderPage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosHomeScreenFolderPage resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|apps|[iosHomeScreenApp](../resources/ioshomescreenapp.md) collection|A list of apps to appear on a page within a folder. This collection can contain a maximum of 500 elements.|
|displayName|String|Name of the folder page|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "bundleID": "String"
    }
  ]
}
```

