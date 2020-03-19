---
title: "validateProperties"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# validateProperties

Namespace: microsoft.graph



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
POST /groups/{groupsId}/validateProperties
POST /me/joinedTeams/{groupId}/validateProperties
POST /users/{usersId}/joinedTeams/{groupId}/validateProperties
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|mailNickname|String||
|onBehalfOfUserId|Guid||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groups/{groupsId}/validateProperties

Content-type: application/json
Content-length: 148

{
  "displayName": "Display Name value",
  "mailNickname": "Mail Nickname value",
  "onBehalfOfUserId": "c2e9f8d9-f8d9-c2e9-d9f8-e9c2d9f8e9c2"
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
HTTP/1.1 204 No Content
```

