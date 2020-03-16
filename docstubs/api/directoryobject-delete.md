---
title: "Delete directoryObject"
description: "Deletes a directoryObject."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete directoryObject

Namespace: microsoft.graph

Deletes a [directoryObject](../resources/directoryobject.md).

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
DELETE /directoryObjects/{directoryObjectsId}
DELETE /directory/deletedItems/{directoryObjectId}
DELETE /groups/{groupsId}/acceptedSenders/{directoryObjectId}
DELETE /groups/{groupsId}/rejectedSenders/{directoryObjectId}
DELETE /me/joinedTeams/{groupId}/acceptedSenders/{directoryObjectId}
DELETE /me/joinedTeams/{groupId}/rejectedSenders/{directoryObjectId}
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
  "name": "delete_directoryobject"
}
-->
``` http
DELETE https://graph.microsoft.com/localtest/directoryObjects/{directoryObjectsId}
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

