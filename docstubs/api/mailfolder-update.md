---
title: "Update mailFolder"
description: "Update the properties of a mailFolder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mailFolder

Namespace: microsoft.graph

Update the properties of a [mailFolder](../resources/mailfolder.md) object.

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
PATCH /me/mailFolders/{mailFolderId}
PATCH /users/{usersId}/mailFolders/{mailFolderId}
PATCH /me/mailFolders/{mailFolderId}/childFolders/{mailFolderId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [mailFolder](../resources/mailfolder.md) object.

The following table shows the properties that are required when you create the [mailFolder](../resources/mailfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|parentFolderId|String||
|childFolderCount|Int32||
|unreadItemCount|Int32||
|totalItemCount|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/mailFolders/{mailFolderId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.mailFolder",
  "displayName": "Display Name value",
  "parentFolderId": "Parent Folder Id value",
  "childFolderCount": 0,
  "unreadItemCount": 15,
  "totalItemCount": 14
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
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.mailFolder",
  "id": "0f6b4dbc-4dbc-0f6b-bc4d-6b0fbc4d6b0f",
  "displayName": "Display Name value",
  "parentFolderId": "Parent Folder Id value",
  "childFolderCount": 0,
  "unreadItemCount": 15,
  "totalItemCount": 14
}
```

