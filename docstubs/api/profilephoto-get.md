---
title: "Get profilePhoto"
description: "Read properties and relationships of the profilePhoto object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get profilePhoto

Namespace: microsoft.graph

Read properties and relationships of the [profilePhoto](../resources/profilephoto.md) object.

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
GET /me/photo
GET /users/{usersId}/photo
GET /groups/{groupsId}/photo
GET /me/photos/{profilePhotoId}
GET /me/contacts/{contactId}/photo
GET /me/joinedTeams/{groupId}/photo
GET /users/{usersId}/photos/{profilePhotoId}
GET /groups/{groupsId}/photos/{profilePhotoId}
GET /me/joinedTeams/{groupId}/photos/{profilePhotoId}
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
If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_profilephoto"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/photo
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": {
    "@odata.type": "#microsoft.graph.profilePhoto",
    "id": "59c1d57e-d57e-59c1-7ed5-c1597ed5c159",
    "height": 6,
    "width": 5
  }
}
```

