---
title: "iosHomeScreenPage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosHomeScreenPage resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Name of the page|
|icons|[iosHomeScreenItem](../resources/ioshomescreenitem.md) collection|A list of apps and folders to appear on a page. This collection can contain a maximum of 500 elements.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```

