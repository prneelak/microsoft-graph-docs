---
title: "participant resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# participant resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get participant](../api/participant-get.md)|[participant](../resources/participant.md)|Read properties and relationships of the [participant](../resources/participant.md) object.|
|[Update participant](../api/participant-update.md)|[participant](../resources/participant.md)|Update the properties of a [participant](../resources/participant.md) object.|
|[invite](../api/participant-invite.md)|[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)||
|[mute](../api/participant-mute.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)||
|[List participants](../api/call-list-participants.md)|[participant](../resources/participant.md) collection|Get the participants from the participants navigation property.|
|[Add participants](../api/call-post-participants.md)|[participant](../resources/participant.md)|Add participants by posting to the participants collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|info|[participantInfo](../resources/participantinfo.md)||
|isInLobby|Boolean||
|isMuted|Boolean||
|mediaStreams|[mediaStream](../resources/mediastream.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.participant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.participant",
  "id": "String (identifier)",
  "info": {
    "@odata.type": "microsoft.graph.participantInfo"
  },
  "mediaStreams": [
    {
      "@odata.type": "microsoft.graph.mediaStream"
    }
  ],
  "isMuted": true,
  "isInLobby": true
}
```

