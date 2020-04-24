---
title: "deviceGeoLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceGeoLocation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|altitude|Double|Altitude, given in meters above sea level|
|heading|Double|Heading in degrees from true north|
|horizontalAccuracy|Double|Accuracy of longitude and latitude in meters|
|lastCollectedDateTime|DateTimeOffset|Time at which location was recorded, relative to UTC|
|lastCollectedDateTimeUtc|DateTimeOffset|Time at which location was recorded, relative to UTC|
|latitude|Double|Latitude coordinate of the device's location|
|longitude|Double|Longitude coordinate of the device's location|
|speed|Double|Speed the device is traveling in meters per second|
|verticalAccuracy|Double|Accuracy of altitude in meters|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "Double",
  "latitude": "Double",
  "altitude": "Double",
  "horizontalAccuracy": "Double",
  "verticalAccuracy": "Double",
  "heading": "Double",
  "speed": "Double"
}
```

