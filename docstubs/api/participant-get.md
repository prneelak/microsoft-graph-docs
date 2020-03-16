---
title: "Get participant"
description: "Read properties and relationships of the participant object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get participant

Namespace: microsoft.graph

Read properties and relationships of the [participant](../resources/participant.md) object.

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
GET /communications/calls/{callId}/participants/{participantId}
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
If successful, this method returns a `200 OK` response code and [participant](../resources/participant.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_participant"
}
-->
``` http
GET https://graph.microsoft.com/localtest/communications/calls/{callId}/participants/{participantId}
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1018

{
  "value": {
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
}
```

