---
title: "Add columnLinks"
description: "Add columnLinks by posting to the columnLinks collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add columnLinks

Namespace: microsoft.graph

Add columnLinks by posting to the columnLinks collection.

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
POST /me/joinedGroups/{groupId}/drive/list/contentTypes/{contentTypeId}/columnLinks/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [columnLink](../resources/columnlink.md) object.

The following table shows the properties that are required when you create the [columnLink](../resources/columnlink.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||



## Response
If successful, this method returns a `201 Created` response code and a [columnLink](../resources/columnlink.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_columnlink_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/list/contentTypes/{contentTypeId}/columnLinks
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.columnLink",
  "name": "Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnlink"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.columnLink",
  "id": "f01c274b-274b-f01c-4b27-1cf04b271cf0",
  "name": "Name value"
}
```

