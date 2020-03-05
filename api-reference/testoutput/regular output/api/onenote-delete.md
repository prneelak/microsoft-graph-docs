---
title: "Delete onenote"
description: "Deletes a onenote."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete onenote

Namespace: microsoft.graph

Deletes a [onenote](../resources/onenote.md).

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
DELETE /me/onenote
DELETE /users/{usersId}/onenote
DELETE /sites/{sitesId}/onenote
DELETE /groups/{groupsId}/onenote
DELETE /me/joinedTeams/{groupId}/onenote
DELETE /me/joinedTeams/{groupId}/sites/{siteId}/onenote
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_onenote"
}
-->
``` http
DELETE https://graph.microsoft.com/localtest/me/onenote
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

