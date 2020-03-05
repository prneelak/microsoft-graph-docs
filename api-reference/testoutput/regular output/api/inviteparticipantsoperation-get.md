---
title: "Get inviteParticipantsOperation"
description: "Read properties and relationships of the inviteParticipantsOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get inviteParticipantsOperation

Namespace: microsoft.graph

Read properties and relationships of the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) object.

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
GET ** Entity URI for microsoft.graph.inviteParticipantsOperation not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_inviteparticipantsoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.inviteParticipantsOperation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1066

{
  "value": {
    "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
    "id": "cf6aee6c-ee6c-cf6a-6cee-6acf6cee6acf",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.resultInfo",
      "code": 4,
      "subcode": 7,
      "message": "Message value"
    },
    "participants": [
      {
        "@odata.type": "microsoft.graph.invitationParticipantInfo",
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
        "languageId": "Language Id value",
        "replacesCallId": "Replaces Call Id value"
      }
    ]
  }
}
```

