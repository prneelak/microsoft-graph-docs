---
title: "Update channel"
description: "Update the properties of a channel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update channel

Namespace: microsoft.graph

Update the properties of a [channel](../resources/channel.md) object.

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
PATCH /teams/{teamsId}/channels/{channelId}
PATCH /me/joinedTeams/{groupId}/team/channels/{channelId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [channel](../resources/channel.md) object.

The following table shows the properties that are required when you create the [channel](../resources/channel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|email|String||
|webUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [channel](../resources/channel.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_channel"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/teams/{teamsId}/channels/{channelId}
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.channel",
  "displayName": "Display Name value",
  "description": "Description value",
  "email": "Email value",
  "webUrl": "https://example.com/webUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.type": "#microsoft.graph.channel",
  "id": "3ac3eb7a-eb7a-3ac3-7aeb-c33a7aebc33a",
  "displayName": "Display Name value",
  "description": "Description value",
  "email": "Email value",
  "webUrl": "https://example.com/webUrl/"
}
```

