---
title: "daylightTimeZoneOffset resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# daylightTimeZoneOffset resource type


Namespace: microsoft.graph




Inherits from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|daylightBias|Int32||
|dayOccurrence|Int32| Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|
|dayOfWeek|Enumeration| Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md). Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|month|Int32| Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|
|time|TimeOfDay| Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|
|year|Int32| Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.daylightTimeZoneOffset",
  "time": "String (time of day)",
  "dayOccurrence": 1024,
  "dayOfWeek": "String",
  "month": 1024,
  "year": 1024,
  "daylightBias": 1024
}
```

