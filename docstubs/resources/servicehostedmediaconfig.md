---
title: "serviceHostedMediaConfig resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# serviceHostedMediaConfig resource type


Namespace: microsoft.graph




Inherits from [mediaConfig](../resources/mediaconfig.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|preFetchMedia|[mediaInfo](../resources/mediainfo.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
  "preFetchMedia": [
    {
      "@odata.type": "microsoft.graph.mediaInfo",
      "uri": "String",
      "resourceId": "String"
    }
  ]
}
```

