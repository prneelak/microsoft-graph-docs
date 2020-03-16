---
title: "onPremisesProvisioningError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onPremisesProvisioningError resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|String||
|occurredDateTime|DateTimeOffset||
|propertyCausingError|String||
|value|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesProvisioningError",
  "value": "String",
  "category": "String",
  "propertyCausingError": "String",
  "occurredDateTime": "String (timestamp)"
}
```

