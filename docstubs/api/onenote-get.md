---
title: "Get onenote"
description: "Read properties and relationships of the onenote object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onenote

Namespace: microsoft.graph

Read properties and relationships of the [onenote](../resources/onenote.md) object.

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
GET /me/onenote
GET /users/{usersId}/onenote
GET /sites/{sitesId}/onenote
GET /groups/{groupsId}/onenote
GET /me/joinedTeams/{groupId}/onenote
GET /me/joinedTeams/{groupId}/sites/{siteId}/onenote
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [onenote](../resources/onenote.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenote"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/onenote
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenote"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 121

{
  "value": {
    "@odata.type": "#microsoft.graph.onenote",
    "id": "e56069e7-69e7-e560-e769-60e5e76960e5"
  }
}
```

