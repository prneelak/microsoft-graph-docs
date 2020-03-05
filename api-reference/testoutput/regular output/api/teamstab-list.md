---
title: "List teamsTabs"
description: "List properties and relationships of the teamsTab objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List teamsTabs

Namespace: microsoft.graph

List properties and relationships of the [teamsTab](../resources/teamstab.md) objects.

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
GET /me/joinedTeams/{groupId}/team/channels/{channelId}/tabs
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsTab](../resources/teamstab.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamstab"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/team/channels/{channelId}/tabs
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamstab)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 544

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsTab",
      "id": "2110d502-d502-2110-02d5-102102d51021",
      "displayName": "Display Name value",
      "webUrl": "https://example.com/webUrl/",
      "configuration": {
        "@odata.type": "microsoft.graph.teamsTabConfiguration",
        "entityId": "Entity Id value",
        "contentUrl": "https://example.com/contentUrl/",
        "removeUrl": "https://example.com/removeUrl/",
        "websiteUrl": "https://example.com/websiteUrl/"
      }
    }
  ]
}
```

