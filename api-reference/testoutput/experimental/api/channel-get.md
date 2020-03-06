---
title: "Get channel"
description: "Read properties and relationships of the channel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get channel

Namespace: microsoft.graph

Read properties and relationships of the [channel](../resources/channel.md) object.

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
GET /teams/{teamsId}/primaryChannel
GET /teams/{teamsId}/channels/{channelId}
GET /me/joinedGroups/{groupId}/team/primaryChannel
GET /me/joinedGroups/{groupId}/team/channels/{channelId}
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
If successful, this method returns a `200 OK` response code and [channel](../resources/channel.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_channel"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teams/{teamsId}/primaryChannel
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.channel",
    "id": "2582a55d-a55d-2582-5da5-82255da58225",
    "displayName": "Display Name value",
    "description": "Description value",
    "isFavoriteByDefault": true,
    "email": "Email value",
    "webUrl": "https://example.com/webUrl/",
    "membershipType": "String"
  }
}
```

