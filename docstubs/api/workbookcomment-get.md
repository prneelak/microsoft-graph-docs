---
title: "Get workbookComment"
description: "Read properties and relationships of the workbookComment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbookComment

Namespace: microsoft.graph

Read properties and relationships of the [workbookComment](../resources/workbookcomment.md) object.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/comments/{workbookCommentId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [workbookComment](../resources/workbookcomment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/comments/{workbookCommentId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 204

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookComment",
    "id": "a2d88593-8593-a2d8-9385-d8a29385d8a2",
    "content": "Content value",
    "contentType": "Content Type value"
  }
}
```

