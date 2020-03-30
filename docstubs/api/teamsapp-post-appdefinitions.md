---
title: "Create appDefinitions"
description: "Create appDefinitions by posting to the appDefinitions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create appDefinitions

Namespace: microsoft.graph

Create appDefinitions by posting to the appDefinitions collection.

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
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [teamsAppDefinition](../resources/teamsappdefinition.md) object.

The following table shows the properties that are required when you create the [teamsAppDefinition](../resources/teamsappdefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|teamsAppId|String||
|displayName|String||
|version|String||



## Response
If successful, this method returns a `201 Created` response code and a [teamsAppDefinition](../resources/teamsappdefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsappdefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "teamsAppId": "Teams App Id value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsappdefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 219

{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "id": "7b52b024-b024-7b52-24b0-527b24b0527b",
  "teamsAppId": "Teams App Id value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

