---
title: "Add photos"
description: "Add photos by posting to the photos collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add photos

Namespace: microsoft.graph

Add photos by posting to the photos collection.

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
POST /me/photos/$ref
POST /users/{usersId}/photos/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [profilePhoto](../resources/profilephoto.md) object.

The following table shows the properties that are required when you create the [profilePhoto](../resources/profilephoto.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|height|Int32||
|width|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [profilePhoto](../resources/profilephoto.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_profilephoto_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/photos
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
  "truncated": true,
  "@odata.type": "microsoft.graph.profilephoto"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 134

{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "id": "59c1d57e-d57e-59c1-7ed5-c1597ed5c159",
  "height": 6,
  "width": 5
}
```

