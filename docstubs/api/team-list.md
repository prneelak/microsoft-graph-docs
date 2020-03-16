---
title: "List teams"
description: "List properties and relationships of the team objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List teams

Namespace: microsoft.graph

List properties and relationships of the [team](../resources/team.md) objects.

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
GET /teams
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
If successful, this method returns a `200 OK` response code and a collection of [team](../resources/team.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_team"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teams
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.team)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1163

{
  "value": [
    {
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
  ]
}
```

