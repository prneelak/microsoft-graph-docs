---
title: "Update profilePhoto"
description: "Update the properties of a profilePhoto object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update profilePhoto

Namespace: microsoft.graph

Update the properties of a [profilePhoto](../resources/profilephoto.md) object.

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
PATCH /me/photo
PATCH /users/{usersId}/photo
PATCH /groups/{groupsId}/photo
PATCH /me/photos/{profilePhotoId}
PATCH /me/contacts/{contactId}/photo
PATCH /me/joinedTeams/{groupId}/photo
PATCH /users/{usersId}/photos/{profilePhotoId}
PATCH /groups/{groupsId}/photos/{profilePhotoId}
PATCH /me/joinedTeams/{groupId}/photos/{profilePhotoId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [profilePhoto](../resources/profilephoto.md) object.

The following table shows the properties that are required when you create the [profilePhoto](../resources/profilephoto.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|height|Int32||
|width|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [profilePhoto](../resources/profilephoto.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/photo
Content-type: application/json
Content-length: 85

{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "height": 6,
  "width": 5
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
Content-Length: 134

{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "id": "59c1d57e-d57e-59c1-7ed5-c1597ed5c159",
  "height": 6,
  "width": 5
}
```

