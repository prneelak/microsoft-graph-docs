---
title: "Update teamsAppDefinition"
description: "Update the properties of a teamsAppDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsAppDefinition

Namespace: microsoft.graph

Update the properties of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.

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
PATCH /me/joinedTeams/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions/{teamsAppDefinitionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [teamsAppDefinition](../resources/teamsappdefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsappdefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions/{teamsAppDefinitionId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 219

{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "id": "8c3c15fe-15fe-8c3c-fe15-3c8cfe153c8c",
  "teamsAppId": "Teams App Id value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

