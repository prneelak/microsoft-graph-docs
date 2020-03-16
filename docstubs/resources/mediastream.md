---
title: "mediaStream resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mediaStream resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|direction|Enumeration|. Possible values are: `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.|
|label|String||
|mediaType|Enumeration|. Possible values are: `audio`, `video`, `videoBasedScreenSharing`, `data`, `unknownFutureValue`.|
|serverMuted|Boolean||
|sourceId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaStream"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaStream",
  "mediaType": "String",
  "label": "String",
  "sourceId": "String",
  "direction": "String",
  "serverMuted": true
}
```

