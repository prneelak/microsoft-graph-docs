---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

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
GET /me/mailFolders/delta
GET /users/{usersId}/mailFolders/delta
GET /me/mailFolders/{mailFolderId}/childFolders/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [mailFolder](../resources/mailfolder.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/mailFolders/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mailfolder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailFolder",
      "id": "0f6b4dbc-4dbc-0f6b-bc4d-6b0fbc4d6b0f",
      "displayName": "Display Name value",
      "parentFolderId": "Parent Folder Id value",
      "childFolderCount": 0,
      "unreadItemCount": 15,
      "totalItemCount": 14
    }
  ]
}
```

