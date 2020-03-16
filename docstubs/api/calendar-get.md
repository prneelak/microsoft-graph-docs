---
title: "Get calendar"
description: "Read properties and relationships of the calendar object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get calendar

Namespace: microsoft.graph

Read properties and relationships of the [calendar](../resources/calendar.md) object.

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
GET /me/calendar
GET /users/{usersId}/calendar
GET /me/calendars/{calendarId}
GET /groups/{groupsId}/calendar
GET /me/joinedTeams/{groupId}/calendar
GET /users/{usersId}/calendars/{calendarId}
GET /me/calendarGroups/{calendarGroupId}/calendars/{calendarId}
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar
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
If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/calendar
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 402

{
  "value": {
    "@odata.type": "#microsoft.graph.calendar",
    "id": "6d0994be-94be-6d09-be94-096dbe94096d",
    "name": "Name value",
    "color": "String",
    "changeKey": "Change Key value",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "owner": {
      "@odata.type": "microsoft.graph.emailAddress",
      "address": "Address value"
    }
  }
}
```

