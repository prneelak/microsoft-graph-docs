---
title: "Add items"
description: "Add items by posting to the items collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add items

Namespace: microsoft.graph

Add items by posting to the items collection.

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
POST /sites/{sitesId}/items/$ref
POST /me/joinedTeams/{groupId}/sites/{siteId}/items/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [baseItem](../resources/baseitem.md) object.

The following table shows the properties that are required when you create the [baseItem](../resources/baseitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset||
|description|String||
|eTag|String||
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||
|name|String||
|parentReference|[itemReference](../resources/itemreference.md)||
|webUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [baseItem](../resources/baseitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_baseitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/sites/{sitesId}/items
Content-type: application/json
Content-length: 1101

{
  "@odata.type": "#microsoft.graph.baseItem",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "description": "Description value",
  "eTag": "ETag value",
  "name": "Name value",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
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
  "webUrl": "https://example.com/webUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.baseitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1352

{
  "@odata.type": "#microsoft.graph.baseItem",
  "id": "efee5129-5129-efee-2951-eeef2951eeef",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "description": "Description value",
  "eTag": "ETag value",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "name": "Name value",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "Drive Id value",
    "driveType": "Drive Type value",
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
  "webUrl": "https://example.com/webUrl/"
}
```

