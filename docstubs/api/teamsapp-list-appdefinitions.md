---
title: "List appDefinitions"
description: "Get the teamsAppDefinitions from the appDefinitions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appDefinitions

Namespace: microsoft.graph

Get the teamsAppDefinitions from the appDefinitions navigation property.

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
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsAppDefinition](../resources/teamsappdefinition.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_teamsappdefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}/teamsApp/appDefinitions
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsappdefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsAppDefinition",
      "id": "9a4e8f73-8f73-9a4e-738f-4e9a738f4e9a",
      "teamsAppId": "Teams App Id value",
      "displayName": "Display Name value",
      "version": "Version value"
    }
  ]
}
```

