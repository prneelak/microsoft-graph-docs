---
title: "webApplication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# webApplication resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|homePageUrl|String||
|implicitGrantSettings|[implicitGrantSettings](../resources/implicitgrantsettings.md)||
|logoutUrl|String||
|redirectUris|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.webApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webApplication",
  "homePageUrl": "String",
  "redirectUris": [
    "String"
  ],
  "logoutUrl": "String",
  "implicitGrantSettings": {
    "@odata.type": "microsoft.graph.implicitGrantSettings",
    "enableIdTokenIssuance": true,
    "enableAccessTokenIssuance": true
  }
}
```

