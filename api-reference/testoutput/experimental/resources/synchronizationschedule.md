---
title: "synchronizationSchedule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationSchedule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|expiration|DateTimeOffset||
|interval|Duration||
|state|Enumeration|. Possible values are: `Active`, `Disabled`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchedule",
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}
```

