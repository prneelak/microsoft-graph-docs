---
title: "requiredResourceAccess resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# requiredResourceAccess resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|resourceAccess|[resourceAccess](../resources/resourceaccess.md) collection||
|resourceAppId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requiredResourceAccess",
  "resourceAppId": "String",
  "resourceAccess": [
    {
      "@odata.type": "microsoft.graph.resourceAccess",
      "id": "Guid",
      "type": "String"
    }
  ]
}
```

