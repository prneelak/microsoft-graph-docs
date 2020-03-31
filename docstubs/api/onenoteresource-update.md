---
title: "Update onenoteResource"
description: "Update the properties of a onenoteResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onenoteResource

Namespace: microsoft.graph

Update the properties of a [onenoteResource](../resources/onenoteresource.md) object.

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
PATCH /me/joinedGroups/{groupId}/sites/{siteId}/onenote/resources/{onenoteResourceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [onenoteResource](../resources/onenoteresource.md) object.

The following table shows the properties that are required when you create the [onenoteResource](../resources/onenoteresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|content|Stream||
|contentUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [onenoteResource](../resources/onenoteresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onenoteresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/sites/{siteId}/onenote/resources/{onenoteResourceId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "self": "Self value",
  "content": "Stream",
  "contentUrl": "https://example.com/contentUrl/"
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
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "id": "47890c9d-0c9d-4789-9d0c-89479d0c8947",
  "self": "Self value",
  "content": "Stream",
  "contentUrl": "https://example.com/contentUrl/"
}
```

