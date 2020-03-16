---
title: "Add participants"
description: "Add participants by posting to the participants collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add participants

Namespace: microsoft.graph

Add participants by posting to the participants collection.

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
POST /communications/calls/{callId}/participants/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [participant](../resources/participant.md) object.

The following table shows the properties that are required when you create the [participant](../resources/participant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|info|[participantInfo](../resources/participantinfo.md)||
|mediaStreams|[mediaStream](../resources/mediastream.md) collection||
|isMuted|Boolean||
|isInLobby|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [participant](../resources/participant.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_participant_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/calls/{callId}/participants
Content-type: application/json
Content-length: 884

{
  "@odata.type": "#microsoft.graph.participant",
  "info": {
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
  "mediaStreams": [
    {
      "@odata.type": "microsoft.graph.mediaStream",
      "mediaType": "String",
      "label": "Label value",
      "sourceId": "Source Id value",
      "direction": "String",
      "serverMuted": true
    }
  ],
  "isMuted": true,
  "isInLobby": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.participant",
  "id": "fcc355f7-55f7-fcc3-f755-c3fcf755c3fc",
  "info": {
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
  "mediaStreams": [
    {
      "@odata.type": "microsoft.graph.mediaStream",
      "mediaType": "String",
      "label": "Label value",
      "sourceId": "Source Id value",
      "direction": "String",
      "serverMuted": true
    }
  ],
  "isMuted": true,
  "isInLobby": true
}
```

