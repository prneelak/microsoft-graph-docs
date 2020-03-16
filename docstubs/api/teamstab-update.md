---
title: "Update teamsTab"
description: "Update the properties of a teamsTab object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsTab

Namespace: microsoft.graph

Update the properties of a [teamsTab](../resources/teamstab.md) object.

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
PATCH /me/joinedTeams/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [teamsTab](../resources/teamstab.md) object.

The following table shows the properties that are required when you create the [teamsTab](../resources/teamstab.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|webUrl|String||
|configuration|[teamsTabConfiguration](../resources/teamstabconfiguration.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsTab](../resources/teamstab.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamstab"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}
Content-type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.teamsTab",
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
Content-Length: 467

{
  "@odata.type": "#microsoft.graph.teamsTab",
  "id": "cce7b027-b027-cce7-27b0-e7cc27b0e7cc",
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
```

