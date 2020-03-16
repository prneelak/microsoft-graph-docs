---
title: "findMeetingTimes"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# findMeetingTimes

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
POST /me/findMeetingTimes
POST /users/{usersId}/findMeetingTimes
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
|attendees|[attendeeBase](../resources/attendeebase.md) collection||
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)||
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)||
|meetingDuration|Duration||
|maxCandidates|Int32||
|isOrganizerOptional|Boolean||
|returnSuggestionReasons|Boolean||
|minimumAttendeePercentage|Double||



## Response
If successful, this action returns a `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/findMeetingTimes

Content-type: application/json
Content-length: 775

{
  "attendees": [
    {
      "@odata.type": "microsoft.graph.attendeeBase"
    }
  ],
  "locationConstraint": {
    "@odata.type": "microsoft.graph.locationConstraint",
    "locations": [
      {
        "@odata.type": "microsoft.graph.locationConstraintItem",
        "resolveAvailability": true
      }
    ],
    "isRequired": true,
    "suggestLocation": true
  },
  "timeConstraint": {
    "@odata.type": "microsoft.graph.timeConstraint",
    "activityDomain": "String",
    "timeSlots": [
      {
        "@odata.type": "microsoft.graph.timeSlot"
      }
    ]
  },
  "meetingDuration": "-PT2M1.4503674S",
  "maxCandidates": 13,
  "isOrganizerOptional": true,
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": "Double"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingtimesuggestionsresult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 90

{
  "value": {
    "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
  }
}
```

