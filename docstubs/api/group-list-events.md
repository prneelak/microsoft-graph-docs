---
title: "List events"
description: "Get the events from the events navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List events

Namespace: microsoft.graph

Get the events from the events navigation property.

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
GET /groups/{groupsId}/events
GET /me/joinedTeams/{groupId}/events
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_event"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/events
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.event)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3982

{
  "value": [
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
  ]
}
```

