---
title: "Get team"
description: "Read properties and relationships of the team object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get team

Namespace: microsoft.graph

Read properties and relationships of the [team](../resources/team.md) object.

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
GET /teams/{teamsId}
GET /groups/{groupsId}/team
GET /me/joinedTeams/{groupId}/team
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
If successful, this method returns a `200 OK` response code and [team](../resources/team.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_team"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teams/{teamsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1089

{
  "value": {
    "@odata.type": "#microsoft.graph.team",
    "id": "84b33128-3128-84b3-2831-b3842831b384",
    "webUrl": "https://example.com/webUrl/",
    "memberSettings": {
      "@odata.type": "microsoft.graph.teamMemberSettings",
      "allowCreateUpdateChannels": true,
      "allowDeleteChannels": true,
      "allowAddRemoveApps": true,
      "allowCreateUpdateRemoveTabs": true,
      "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
      "@odata.type": "microsoft.graph.teamGuestSettings"
    },
    "messagingSettings": {
      "@odata.type": "microsoft.graph.teamMessagingSettings",
      "allowUserEditMessages": true,
      "allowUserDeleteMessages": true,
      "allowOwnerDeleteMessages": true,
      "allowTeamMentions": true,
      "allowChannelMentions": true
    },
    "funSettings": {
      "@odata.type": "microsoft.graph.teamFunSettings",
      "allowGiphy": true,
      "giphyContentRating": "String",
      "allowStickersAndMemes": true,
      "allowCustomMemes": true
    },
    "isArchived": true
  }
}
```

