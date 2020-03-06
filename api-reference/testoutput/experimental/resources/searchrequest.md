---
title: "searchRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# searchRequest resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentSources|String collection||
|enableTopResults|Boolean||
|entityTypes|Enumeration collection||
|from|Int32||
|query|[searchQuery](../resources/searchquery.md)||
|size|Int32||
|stored_fields|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchRequest",
  "entityTypes": [
    "String"
  ],
  "contentSources": [
    "String"
  ],
  "query": {
    "@odata.type": "microsoft.graph.searchQuery",
    "query_string": {
      "@odata.type": "microsoft.graph.searchQueryString",
      "query": "String"
    }
  },
  "from": 1024,
  "size": 1024,
  "stored_fields": [
    "String"
  ],
  "enableTopResults": true
}
```

