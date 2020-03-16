---
title: "Update calendar"
description: "Update the properties of a calendar object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update calendar

Namespace: microsoft.graph

Update the properties of a [calendar](../resources/calendar.md) object.

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
PATCH /me/calendar
PATCH /users/{usersId}/calendar
PATCH /me/calendars/{calendarId}
PATCH /groups/{groupsId}/calendar
PATCH /me/joinedTeams/{groupId}/calendar
PATCH /users/{usersId}/calendars/{calendarId}
PATCH /me/calendarGroups/{calendarGroupId}/calendars/{calendarId}
PATCH /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [calendar](../resources/calendar.md) object.

The following table shows the properties that are required when you create the [calendar](../resources/calendar.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|color|Enumeration|. Possible values are: `lightBlue`, `lightGreen`, `lightOrange`, `lightGray`, `lightYellow`, `lightTeal`, `lightPink`, `lightBrown`, `lightRed`, `maxColor`, `auto`.|
|changeKey|String||
|canShare|Boolean||
|canViewPrivateItems|Boolean||
|canEdit|Boolean||
|owner|[emailAddress](../resources/emailaddress.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [calendar](../resources/calendar.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_calendar"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/calendar
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.calendar",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
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
```

