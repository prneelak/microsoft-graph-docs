---
title: "Delete drive"
description: "Deletes a drive."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete drive

Namespace: microsoft.graph

Deletes a [drive](../resources/drive.md).

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
DELETE /drive
DELETE /me/drive
DELETE /drives/{drivesId}
DELETE /me/drive/list/drive
DELETE /me/drives/{driveId}
DELETE /users/{usersId}/drive
DELETE /sites/{sitesId}/drive
DELETE /groups/{groupsId}/drive
DELETE /me/joinedTeams/{groupId}/drive
DELETE /users/{usersId}/drives/{driveId}
DELETE /sites/{sitesId}/drives/{driveId}
DELETE /groups/{groupsId}/drives/{driveId}
DELETE /me/joinedTeams/{groupId}/drives/{driveId}
DELETE /me/joinedTeams/{groupId}/sites/{siteId}/drive
DELETE /me/joinedTeams/{groupId}/sites/{siteId}/drives/{driveId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_drive"
}
-->
``` http
DELETE https://graph.microsoft.com/localtest/drive
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

