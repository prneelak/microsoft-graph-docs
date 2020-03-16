---
title: "standardTimeZoneOffset resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# standardTimeZoneOffset resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|dayOccurrence|Int32||
|dayOfWeek|Enumeration|. Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|month|Int32||
|time|TimeOfDay||
|year|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.standardTimeZoneOffset",
  "time": "String (time of day)",
  "dayOccurrence": 1024,
  "dayOfWeek": "String",
  "month": 1024,
  "year": 1024
}
```

