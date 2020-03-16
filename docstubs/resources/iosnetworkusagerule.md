---
title: "iosNetworkUsageRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosNetworkUsageRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|cellularDataBlocked|Boolean|If set to true, corresponding managed apps will not be allowed to use cellular data at any time.|
|cellularDataBlockWhenRoaming|Boolean|If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.|
|managedApps|[appListItem](../resources/applistitem.md) collection|Information about the managed apps that this rule is going to apply to. This collection can contain a maximum of 500 elements.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```

