---
title: "meetingTimeSuggestionsResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# meetingTimeSuggestionsResult resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|emptySuggestionsReason|String||
|meetingTimeSuggestions|[meetingTimeSuggestion](../resources/meetingtimesuggestion.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingTimeSuggestionsResult",
  "meetingTimeSuggestions": [
    {
      "@odata.type": "microsoft.graph.meetingTimeSuggestion",
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
  ],
  "emptySuggestionsReason": "String"
}
```

