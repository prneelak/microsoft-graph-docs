---
title: "Update call"
description: "Update the properties of a call object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update call

Namespace: microsoft.graph

Update the properties of a [call](../resources/call.md) object.

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
PATCH /communications/calls/{callId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [call](../resources/call.md) object.

The following table shows the properties that are required when you create the [call](../resources/call.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|state|Enumeration|. Possible values are: `incoming`, `establishing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|mediaState|[callMediaState](../resources/callmediastate.md)||
|resultInfo|[resultInfo](../resources/resultinfo.md)||
|direction|Enumeration|. Possible values are: `incoming`, `outgoing`.|
|subject|String||
|callbackUri|String||
|source|[participantInfo](../resources/participantinfo.md)||
|targets|[participantInfo](../resources/participantinfo.md) collection||
|requestedModalities|Enumeration collection|. Possible values are: `audio`, `video`, `videoBasedScreenSharing`, `data`, `unknownFutureValue`.|
|mediaConfig|[mediaConfig](../resources/mediaconfig.md)||
|chatInfo|[chatInfo](../resources/chatinfo.md)||
|meetingInfo|[meetingInfo](../resources/meetinginfo.md)||
|tenantId|String||
|myParticipantId|String||
|toneInfo|[toneInfo](../resources/toneinfo.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [call](../resources/call.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_call"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/communications/calls/{callId}
Content-type: application/json
Content-length: 1645

{
  "@odata.type": "#microsoft.graph.call",
  "state": "String",
  "mediaState": {
    "@odata.type": "microsoft.graph.callMediaState",
    "audio": "String"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "direction": "String",
  "subject": "Subject value",
  "callbackUri": "Callback Uri value",
  "source": {
    "@odata.type": "microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "displayName": "Display Name value",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "region": "Region value",
    "languageId": "Language Id value"
  },
  "targets": [
    {
      "@odata.type": "microsoft.graph.participantInfo"
    }
  ],
  "requestedModalities": [
    "String"
  ],
  "mediaConfig": {
    "@odata.type": "microsoft.graph.mediaConfig"
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo",
    "threadId": "Thread Id value",
    "messageId": "Message Id value",
    "replyChainMessageId": "Reply Chain Message Id value"
  },
  "meetingInfo": {
    "@odata.type": "microsoft.graph.meetingInfo"
  },
  "tenantId": "Tenant Id value",
  "myParticipantId": "My Participant Id value",
  "toneInfo": {
    "@odata.type": "microsoft.graph.toneInfo",
    "sequenceId": 10,
    "tone": "String"
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
Content-Length: 1694

{
  "@odata.type": "#microsoft.graph.call",
  "id": "6825993b-993b-6825-3b99-25683b992568",
  "state": "String",
  "mediaState": {
    "@odata.type": "microsoft.graph.callMediaState",
    "audio": "String"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "direction": "String",
  "subject": "Subject value",
  "callbackUri": "Callback Uri value",
  "source": {
    "@odata.type": "microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "displayName": "Display Name value",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "region": "Region value",
    "languageId": "Language Id value"
  },
  "targets": [
    {
      "@odata.type": "microsoft.graph.participantInfo"
    }
  ],
  "requestedModalities": [
    "String"
  ],
  "mediaConfig": {
    "@odata.type": "microsoft.graph.mediaConfig"
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo",
    "threadId": "Thread Id value",
    "messageId": "Message Id value",
    "replyChainMessageId": "Reply Chain Message Id value"
  },
  "meetingInfo": {
    "@odata.type": "microsoft.graph.meetingInfo"
  },
  "tenantId": "Tenant Id value",
  "myParticipantId": "My Participant Id value",
  "toneInfo": {
    "@odata.type": "microsoft.graph.toneInfo",
    "sequenceId": 10,
    "tone": "String"
  }
}
```

