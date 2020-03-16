---
title: "Add contactFolders"
description: "Add contactFolders by posting to the contactFolders collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add contactFolders

Namespace: microsoft.graph

Add contactFolders by posting to the contactFolders collection.

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
POST /me/contactFolders/$ref
POST /users/{usersId}/contactFolders/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [contactFolder](../resources/contactfolder.md) object.

The following table shows the properties that are required when you create the [contactFolder](../resources/contactfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|parentFolderId|String||
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [contactFolder](../resources/contactfolder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/contactFolders
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.contactFolder",
  "parentFolderId": "Parent Folder Id value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactfolder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 191

{
  "@odata.type": "#microsoft.graph.contactFolder",
  "id": "02b1a6a2-a6a2-02b1-a2a6-b102a2a6b102",
  "parentFolderId": "Parent Folder Id value",
  "displayName": "Display Name value"
}
```

