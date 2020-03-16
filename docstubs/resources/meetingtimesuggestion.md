---
title: "meetingTimeSuggestion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# meetingTimeSuggestion resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendeeAvailability|[attendeeAvailability](../resources/attendeeavailability.md) collection||
|confidence|Double||
|locations|[location](../resources/location.md) collection||
|meetingTimeSlot|[timeSlot](../resources/timeslot.md)||
|order|Int32||
|organizerAvailability|Enumeration|. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|suggestionReason|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingTimeSuggestion",
  "confidence": "Double",
  "order": 1024,
  "organizerAvailability": "String",
  "attendeeAvailability": [
    {
      "@odata.type": "microsoft.graph.attendeeAvailability",
      "attendee": {
        "@odata.type": "microsoft.graph.attendeeBase",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "name": "String",
          "address": "String"
        },
        "type": "String"
      },
      "availability": "String"
    }
  ],
  "locations": [
    {
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
    }
  ],
  "suggestionReason": "String",
  "meetingTimeSlot": {
    "@odata.type": "microsoft.graph.timeSlot",
    "start": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "end": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    }
  }
}
```

