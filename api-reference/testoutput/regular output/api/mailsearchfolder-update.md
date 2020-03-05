---
title: "Update mailSearchFolder"
description: "Update the properties of a mailSearchFolder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mailSearchFolder

Namespace: microsoft.graph

Update the properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.

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
PATCH ** Entity URI for microsoft.graph.mailSearchFolder not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [mailSearchFolder](../resources/mailsearchfolder.md) object.

The following table shows the properties that are required when you create the [mailSearchFolder](../resources/mailsearchfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [mailFolder](../resources/mailfolder.md)|
|parentFolderId|String| Inherited from [mailFolder](../resources/mailfolder.md)|
|childFolderCount|Int32| Inherited from [mailFolder](../resources/mailfolder.md)|
|unreadItemCount|Int32| Inherited from [mailFolder](../resources/mailfolder.md)|
|totalItemCount|Int32| Inherited from [mailFolder](../resources/mailfolder.md)|
|isSupported|Boolean||
|includeNestedFolders|Boolean||
|sourceFolderIds|String collection||
|filterQuery|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.mailSearchFolder not found
Content-type: application/json
Content-length: 380

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "displayName": "Display Name value",
  "parentFolderId": "Parent Folder Id value",
  "childFolderCount": 0,
  "unreadItemCount": 15,
  "totalItemCount": 14,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "Source Folder Ids value"
  ],
  "filterQuery": "Filter Query value"
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
Content-Length: 429

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "41eebc68-bc68-41ee-68bc-ee4168bcee41",
  "displayName": "Display Name value",
  "parentFolderId": "Parent Folder Id value",
  "childFolderCount": 0,
  "unreadItemCount": 15,
  "totalItemCount": 14,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "Source Folder Ids value"
  ],
  "filterQuery": "Filter Query value"
}
```

