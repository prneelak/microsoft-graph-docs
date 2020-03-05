---
title: "Get mailSearchFolder"
description: "Read properties and relationships of the mailSearchFolder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mailSearchFolder

Namespace: microsoft.graph

Read properties and relationships of the [mailSearchFolder](../resources/mailsearchfolder.md) object.

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
GET ** Entity URI for microsoft.graph.mailSearchFolder not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [mailSearchFolder](../resources/mailsearchfolder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mailsearchfolder"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.mailSearchFolder not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": {
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
}
```

