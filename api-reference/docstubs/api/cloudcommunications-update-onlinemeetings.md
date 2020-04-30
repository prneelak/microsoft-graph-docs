---
title: "Update onlineMeetings"
description: "Update the properties of an onlineMeetings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update onlineMeetings

Namespace: microsoft.graph

Update the properties of an onlineMeetings object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /communications/onlineMeetings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.

The following table shows the properties that are required when you create the [onlineMeeting](../resources/onlinemeeting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|canceledDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|entryExitAnnouncement|Boolean|**TODO: Add Description**|
|joinUrl|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|isCancelled|Boolean|**TODO: Add Description**|
|participants|[meetingParticipants](../resources/meetingparticipants.md)|**TODO: Add Description**|
|isBroadcast|Boolean|**TODO: Add Description**|
|accessLevel|accessLevel|**TODO: Add Description**. Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `sameEnterpriseAndFederated`.|
|capabilities|meetingCapabilities collection|**TODO: Add Description**. Possible values are: `questionAndAnswer`, `unknownFutureValue`.|
|audioConferencing|[audioConferencing](../resources/audioconferencing.md)|**TODO: Add Description**|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|videoTeleconferenceId|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|joinInformation|[itemBody](../resources/itembody.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [onlineMeeting](../resources/onlinemeeting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_onlinemeetings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/communications/onlineMeetings
Content-Type: application/json
Content-length: 873

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "canceledDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "entryExitAnnouncement": "Boolean",
  "joinUrl": "String",
  "subject": "String",
  "isCancelled": "Boolean",
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants"
  },
  "isBroadcast": "Boolean",
  "accessLevel": "String",
  "capabilities": [
    "String"
  ],
  "audioConferencing": {
    "@odata.type": "microsoft.graph.audioConferencing"
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo"
  },
  "videoTeleconferenceId": "String",
  "externalId": "String",
  "joinInformation": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "id": "8c5883c3-83c3-8c58-c383-588cc383588c",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "canceledDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "entryExitAnnouncement": "Boolean",
  "joinUrl": "String",
  "subject": "String",
  "isCancelled": "Boolean",
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants"
  },
  "isBroadcast": "Boolean",
  "accessLevel": "String",
  "capabilities": [
    "String"
  ],
  "audioConferencing": {
    "@odata.type": "microsoft.graph.audioConferencing"
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo"
  },
  "videoTeleconferenceId": "String",
  "externalId": "String",
  "joinInformation": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

