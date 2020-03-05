---
title: "List contactFolders"
description: "List properties and relationships of the contactFolder objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List contactFolders

Namespace: microsoft.graph

List properties and relationships of the [contactFolder](../resources/contactfolder.md) objects.

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
GET /me/contactFolders
GET /users/{usersId}/contactFolders
GET /me/contactFolders/{contactFolderId}/childFolders
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [contactFolder](../resources/contactfolder.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/contactFolders
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.contactfolder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contactFolder",
      "id": "babbdd61-dd61-babb-61dd-bbba61ddbbba",
      "parentFolderId": "Parent Folder Id value",
      "displayName": "Display Name value"
    }
  ]
}
```

