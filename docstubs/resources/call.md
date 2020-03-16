---
title: "call resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# call resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get call](../api/call-get.md)|[call](../resources/call.md)|Read properties and relationships of the [call](../resources/call.md) object.|
|[Update call](../api/call-update.md)|[call](../resources/call.md)|Update the properties of a [call](../resources/call.md) object.|
|[answer](../api/call-answer.md)|None||
|[changeScreenSharingRole](../api/call-changescreensharingrole.md)|None||
|[mute](../api/call-mute.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)||
|[playPrompt](../api/call-playprompt.md)|[playPromptOperation](../resources/playpromptoperation.md)||
|[record](../api/call-record.md)|[recordOperation](../resources/recordoperation.md)||
|[redirect](../api/call-redirect.md)|None||
|[reject](../api/call-reject.md)|None||
|[subscribeToTone](../api/call-subscribetotone.md)|[subscribeToToneOperation](../resources/subscribetotoneoperation.md)||
|[transfer](../api/call-transfer.md)|None||
|[unmute](../api/call-unmute.md)|[unmuteParticipantOperation](../resources/unmuteparticipantoperation.md)||
|[List participants](../api/call-list-participants.md)|[participant](../resources/participant.md) collection|Get the participants from the participants navigation property.|
|[Add participants](../api/call-post-participants.md)|[participant](../resources/participant.md)|Add participants by posting to the participants collection.|
|[List operations](../api/call-list-operations.md)|[commsOperation](../resources/commsoperation.md) collection|Get the commsOperations from the operations navigation property.|
|[Add operations](../api/call-post-operations.md)|[commsOperation](../resources/commsoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callbackUri|String||
|chatInfo|[chatInfo](../resources/chatinfo.md)||
|direction|Enumeration|. Possible values are: `incoming`, `outgoing`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|mediaConfig|[mediaConfig](../resources/mediaconfig.md)||
|mediaState|[callMediaState](../resources/callmediastate.md)||
|meetingInfo|[meetingInfo](../resources/meetinginfo.md)||
|myParticipantId|String||
|requestedModalities|Enumeration collection||
|resultInfo|[resultInfo](../resources/resultinfo.md)||
|source|[participantInfo](../resources/participantinfo.md)||
|state|Enumeration|. Possible values are: `incoming`, `establishing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|subject|String||
|targets|[participantInfo](../resources/participantinfo.md) collection||
|tenantId|String||
|toneInfo|[toneInfo](../resources/toneinfo.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|operations|[commsOperation](../resources/commsoperation.md) collection||
|participants|[participant](../resources/participant.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.call",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.call",
  "id": "String (identifier)",
  "state": "String",
  "mediaState": {
    "@odata.type": "microsoft.graph.callMediaState",
    "audio": "String"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "direction": "String",
  "subject": "String",
  "callbackUri": "String",
  "source": {
    "@odata.type": "microsoft.graph.participantInfo"
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
    "threadId": "String",
    "messageId": "String",
    "replyChainMessageId": "String"
  },
  "meetingInfo": {
    "@odata.type": "microsoft.graph.meetingInfo"
  },
  "tenantId": "String",
  "myParticipantId": "String",
  "toneInfo": {
    "@odata.type": "microsoft.graph.toneInfo",
    "sequenceId": 1024,
    "tone": "String"
  }
}
```

