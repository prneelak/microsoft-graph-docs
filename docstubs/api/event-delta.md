---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /me/events/delta
GET /me/calendarView/delta
GET /users/{usersId}/events/delta
GET /groups/{groupsId}/events/delta
GET /users/{usersId}/calendarView/delta
GET /groups/{groupsId}/calendarView/delta
GET /me/joinedTeams/{groupId}/events/delta
GET /me/joinedTeams/{groupId}/calendarView/delta
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/instances/delta
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/events/delta
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/calendarView/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [event](../resources/event.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "event_delta"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/events/delta
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
Content-Length: 1977

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
        "@odata.type": "microsoft.graph.responseStatus"
      },
      "iCalUId": "ICal UId value",
      "reminderMinutesBeforeStart": 10,
      "isReminderOn": true,
      "hasAttachments": true,
      "subject": "Subject value",
      "body": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "bodyPreview": "Body Preview value",
      "importance": "String",
      "sensitivity": "String",
      "start": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "originalStart": "2017-01-01T00:01:30.674817+03:00",
      "end": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "location": {
        "@odata.type": "microsoft.graph.location"
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
        "@odata.type": "microsoft.graph.patternedRecurrence"
      },
      "responseRequested": true,
      "seriesMasterId": "Series Master Id value",
      "showAs": "String",
      "type": "String",
      "attendees": [
        {
          "@odata.type": "microsoft.graph.attendee"
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

