---
title: "snoozeReminder"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# snoozeReminder

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
POST /me/events/{eventId}/snoozeReminder
POST /me/calendarView/{eventId}/snoozeReminder
POST /users/{usersId}/events/{eventId}/snoozeReminder
POST /groups/{groupsId}/events/{eventId}/snoozeReminder
POST /users/{usersId}/calendarView/{eventId}/snoozeReminder
POST /groups/{groupsId}/calendarView/{eventId}/snoozeReminder
POST /me/joinedTeams/{groupId}/events/{eventId}/snoozeReminder
POST /me/joinedTeams/{groupId}/calendarView/{eventId}/snoozeReminder
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/snoozeReminder
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/instances/{eventId}/snoozeReminder
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/events/{eventId}/snoozeReminder
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/calendarView/{eventId}/snoozeReminder
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|NewReminderTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/events/{eventId}/snoozeReminder

Content-type: application/json
Content-length: 88

{
  "NewReminderTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

