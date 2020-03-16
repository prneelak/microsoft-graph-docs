---
title: "Update onenote"
description: "Update the properties of a onenote object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onenote

Namespace: microsoft.graph

Update the properties of a [onenote](../resources/onenote.md) object.

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
PATCH /me/onenote
PATCH /users/{usersId}/onenote
PATCH /sites/{sitesId}/onenote
PATCH /groups/{groupsId}/onenote
PATCH /me/joinedTeams/{groupId}/onenote
PATCH /me/joinedTeams/{groupId}/sites/{siteId}/onenote
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [onenote](../resources/onenote.md) object.

The following table shows the properties that are required when you create the [onenote](../resources/onenote.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [onenote](../resources/onenote.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onenote"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/onenote
Content-type: application/json
Content-length: 49

{
  "@odata.type": "#microsoft.graph.onenote"
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
Content-Length: 98

{
  "@odata.type": "#microsoft.graph.onenote",
  "id": "cda0eace-eace-cda0-ceea-a0cdceeaa0cd"
}
```

