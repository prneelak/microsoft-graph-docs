---
title: "Get onlineMeeting"
description: "Read properties and relationships of the onlineMeeting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onlineMeeting

Namespace: microsoft.graph

Read properties and relationships of the [onlineMeeting](../resources/onlinemeeting.md) object.

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
GET /me/onlineMeetings/{onlineMeetingId}
GET /app/onlineMeetings/{onlineMeetingId}
GET /communications/onlineMeetings/{onlineMeetingId}
GET /users/{usersId}/onlineMeetings/{onlineMeetingId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onlinemeeting"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/onlineMeetings/{onlineMeetingId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2467

{
  "value": {
    "@odata.type": "#microsoft.graph.onlineMeeting",
    "id": "45bb6c28-6c28-45bb-286c-bb45286cbb45",
    "creationDateTime": "2017-01-01T00:01:50.3140554+03:00",
    "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
    "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
    "canceledDateTime": "2017-01-01T00:02:39.0139557+03:00",
    "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
    "entryExitAnnouncement": true,
    "joinUrl": "https://example.com/joinUrl/",
    "subject": "Subject value",
    "isCancelled": true,
    "participants": {
      "@odata.type": "microsoft.graph.meetingParticipants",
      "organizer": {
        "@odata.type": "microsoft.graph.meetingParticipantInfo",
        "identity": {
          "@odata.type": "microsoft.graph.identitySet",
          "application": {
            "@odata.type": "microsoft.graph.identity",
            "id": "Id value",
            "displayName": "Display Name value"
          },
          "device": {
            "@odata.type": "microsoft.graph.identity"
          },
          "user": {
            "@odata.type": "microsoft.graph.identity"
          }
        },
        "upn": "Upn value"
      },
      "attendees": [
        {
          "@odata.type": "microsoft.graph.meetingParticipantInfo"
        }
      ],
      "producers": [
        {
          "@odata.type": "microsoft.graph.meetingParticipantInfo"
        }
      ],
      "contributors": [
        {
          "@odata.type": "microsoft.graph.meetingParticipantInfo"
        }
      ]
    },
    "isBroadcast": true,
    "accessLevel": "String",
    "capabilities": [
      "String"
    ],
    "audioConferencing": {
      "@odata.type": "microsoft.graph.audioConferencing",
      "conferenceId": "Conference Id value",
      "tollNumber": "Toll Number value",
      "tollFreeNumber": "Toll Free Number value",
      "dialinUrl": "https://example.com/dialinUrl/"
    },
    "chatInfo": {
      "@odata.type": "microsoft.graph.chatInfo",
      "threadId": "Thread Id value",
      "messageId": "Message Id value",
      "replyChainMessageId": "Reply Chain Message Id value"
    },
    "videoTeleconferenceId": "Video Teleconference Id value",
    "externalId": "External Id value",
    "joinInformation": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    }
  }
}
```

