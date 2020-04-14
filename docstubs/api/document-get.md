---
title: "Get document"
description: "Read properties and relationships of the document object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get document

Namespace: microsoft.graph

Read properties and relationships of the [document](../resources/document.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /workbooks/{workbooksId}/document
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [document](../resources/document.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_document"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/document
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.document"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 122

{
  "value": {
    "@odata.type": "#microsoft.graph.document",
    "id": "3342f921-f921-3342-21f9-423321f94233"
  }
}
```

