---
title: "Add contentTypes"
description: "Add contentTypes by posting to the contentTypes collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add contentTypes

Namespace: microsoft.graph

Add contentTypes by posting to the contentTypes collection.

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
POST /me/drive/list/contentTypes/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [contentType](../resources/contenttype.md) object.

The following table shows the properties that are required when you create the [contentType](../resources/contenttype.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|group|String||
|hidden|Boolean||
|inheritedFrom|[itemReference](../resources/itemreference.md)||
|name|String||
|order|[contentTypeOrder](../resources/contenttypeorder.md)||
|parentId|String||
|readOnly|Boolean||
|sealed|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [contentType](../resources/contenttype.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_contenttype_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/list/contentTypes
Content-type: application/json
Content-length: 952

{
  "@odata.type": "#microsoft.graph.contentType",
  "description": "Description value",
  "group": "Group value",
  "hidden": true,
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "id": "Id value",
    "name": "Name value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "webId": "Web Id value"
    }
  },
  "name": "Name value",
  "order": {
    "@odata.type": "microsoft.graph.contentTypeOrder",
    "default": true,
    "position": 8
  },
  "parentId": "Parent Id value",
  "readOnly": true,
  "sealed": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contenttype"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1001

{
  "@odata.type": "#microsoft.graph.contentType",
  "id": "79bae53a-e53a-79ba-3ae5-ba793ae5ba79",
  "description": "Description value",
  "group": "Group value",
  "hidden": true,
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
    "id": "Id value",
    "name": "Name value",
    "path": "Path value",
    "shareId": "Share Id value",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "List Id value",
      "listItemId": "List Item Id value",
      "listItemUniqueId": "List Item Unique Id value",
      "siteId": "Site Id value",
      "siteUrl": "https://example.com/siteUrl/",
      "webId": "Web Id value"
    }
  },
  "name": "Name value",
  "order": {
    "@odata.type": "microsoft.graph.contentTypeOrder",
    "default": true,
    "position": 8
  },
  "parentId": "Parent Id value",
  "readOnly": true,
  "sealed": true
}
```

