---
title: "Update outlookUser"
description: "Update the properties of a outlookUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update outlookUser

Namespace: microsoft.graph

Update the properties of a [outlookUser](../resources/outlookuser.md) object.

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
PATCH /me/outlook
PATCH /users/{usersId}/outlook
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [outlookUser](../resources/outlookuser.md) object.

The following table shows the properties that are required when you create the [outlookUser](../resources/outlookuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [outlookUser](../resources/outlookuser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_outlookuser"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/outlook
Content-type: application/json
Content-length: 53

{
  "@odata.type": "#microsoft.graph.outlookUser"
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
Content-Length: 102

{
  "@odata.type": "#microsoft.graph.outlookUser",
  "id": "eb8ea100-a100-eb8e-00a1-8eeb00a18eeb"
}
```

