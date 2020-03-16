---
title: "Add events"
description: "Add events by posting to the events collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add events

Namespace: microsoft.graph

Add events by posting to the events collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/events/$ref
POST /users/{usersId}/events/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [event](../resources/event.md) object.

The following table shows the properties that are required when you create the [event](../resources/event.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|originalStartTimeZone|String||
|originalEndTimeZone|String||
|responseStatus|[responseStatus](../resources/responsestatus.md)||
|iCalUId|String||
|reminderMinutesBeforeStart|Int32||
|isReminderOn|Boolean||
|hasAttachments|Boolean||
|subject|String||
|body|[itemBody](../resources/itembody.md)||
|bodyPreview|String||
|importance|Enumeration|. Possible values are: `low`, `normal`, `high`.|
|sensitivity|Enumeration|. Possible values are: `normal`, `personal`, `private`, `confidential`.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|originalStart|DateTimeOffset||
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|location|[location](../resources/location.md)||
|locations|[location](../resources/location.md) collection||
|isAllDay|Boolean||
|isCancelled|Boolean||
|isOrganizer|Boolean||
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)||
|responseRequested|Boolean||
|seriesMasterId|String||
|showAs|Enumeration|. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|type|Enumeration|. Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|attendees|[attendee](../resources/attendee.md) collection||
|organizer|[recipient](../resources/recipient.md)||
|webLink|String||
|onlineMeetingUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [event](../resources/event.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_event_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/events
Content-type: application/json
Content-length: 3313

{
  "@odata.type": "#microsoft.graph.event",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "originalStartTimeZone": "Original Start Time Zone value",
  "originalEndTimeZone": "Original End Time Zone value",
  "responseStatus": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "2017-01-01T00:01:36.132973+03:00"
  },
  "iCalUId": "ICal UId value",
  "reminderMinutesBeforeStart": 10,
  "isReminderOn": true,
  "hasAttachments": true,
  "subject": "Subject value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "bodyPreview": "Body Preview value",
  "importance": "String",
  "sensitivity": "String",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
  },
  "originalStart": "2017-01-01T00:01:30.674817+03:00",
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "location": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "locationUri": "Location Uri value",
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitude": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "locations": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 8,
      "month": 5,
      "dayOfMonth": 10,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "Recurrence Time Zone value",
      "numberOfOccurrences": 3
    }
  },
  "responseRequested": true,
  "seriesMasterId": "Series Master Id value",
  "showAs": "String",
  "type": "String",
  "attendees": [
    {
      "@odata.type": "microsoft.graph.attendee",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      },
      "type": "String",
      "status": {
        "@odata.type": "microsoft.graph.responseStatus"
      }
    }
  ],
  "organizer": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "webLink": "Web Link value",
  "onlineMeetingUrl": "https://example.com/onlineMeetingUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3485

{
  "@odata.type": "#microsoft.graph.event",
  "id": "eab3dfdd-dfdd-eab3-dddf-b3eadddfb3ea",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "originalStartTimeZone": "Original Start Time Zone value",
  "originalEndTimeZone": "Original End Time Zone value",
  "responseStatus": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "2017-01-01T00:01:36.132973+03:00"
  },
  "iCalUId": "ICal UId value",
  "reminderMinutesBeforeStart": 10,
  "isReminderOn": true,
  "hasAttachments": true,
  "subject": "Subject value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "bodyPreview": "Body Preview value",
  "importance": "String",
  "sensitivity": "String",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
  },
  "originalStart": "2017-01-01T00:01:30.674817+03:00",
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "location": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "locationUri": "Location Uri value",
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitude": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "locations": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 8,
      "month": 5,
      "dayOfMonth": 10,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "Recurrence Time Zone value",
      "numberOfOccurrences": 3
    }
  },
  "responseRequested": true,
  "seriesMasterId": "Series Master Id value",
  "showAs": "String",
  "type": "String",
  "attendees": [
    {
      "@odata.type": "microsoft.graph.attendee",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      },
      "type": "String",
      "status": {
        "@odata.type": "microsoft.graph.responseStatus"
      }
    }
  ],
  "organizer": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "webLink": "Web Link value",
  "onlineMeetingUrl": "https://example.com/onlineMeetingUrl/"
}
```

