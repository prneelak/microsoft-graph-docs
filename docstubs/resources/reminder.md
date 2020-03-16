---
title: "reminder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# reminder resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String||
|eventEndTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|eventId|String||
|eventLocation|[location](../resources/location.md)||
|eventStartTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|eventSubject|String||
|eventWebLink|String||
|reminderFireTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.reminder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reminder",
  "eventId": "String",
  "eventStartTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "eventEndTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "changeKey": "String",
  "eventSubject": "String",
  "eventLocation": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "String",
    "locationEmailAddress": "String",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "street": "String",
      "city": "String",
      "state": "String",
      "countryOrRegion": "String",
      "postalCode": "String"
    },
    "locationUri": "String",
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitude": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationType": "String",
    "uniqueId": "String",
    "uniqueIdType": "String"
  },
  "eventWebLink": "String",
  "reminderFireTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

