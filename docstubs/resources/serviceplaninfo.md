---
title: "servicePlanInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# servicePlanInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appliesTo|String||
|provisioningStatus|String||
|servicePlanId|Guid||
|servicePlanName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePlanInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePlanInfo",
  "servicePlanId": "Guid",
  "servicePlanName": "String",
  "provisioningStatus": "String",
  "appliesTo": "String"
}
```

