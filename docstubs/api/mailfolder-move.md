---
title: "move"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# move

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
POST /me/mailFolders/{mailFolderId}/move
POST /users/{usersId}/mailFolders/{mailFolderId}/move
POST /me/mailFolders/{mailFolderId}/childFolders/{mailFolderId}/move
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
|DestinationId|String||



## Response
If successful, this action returns a `200 OK` response code and a [mailFolder](../resources/mailfolder.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/mailFolders/{mailFolderId}/move

Content-type: application/json
Content-length: 47

{
  "DestinationId": "Destination Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailfolder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": {
    "@odata.type": "#microsoft.graph.mailFolder",
    "id": "0f6b4dbc-4dbc-0f6b-bc4d-6b0fbc4d6b0f",
    "displayName": "Display Name value",
    "parentFolderId": "Parent Folder Id value",
    "childFolderCount": 0,
    "unreadItemCount": 15,
    "totalItemCount": 14
  }
}
```

