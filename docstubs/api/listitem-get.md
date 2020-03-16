---
title: "Get listItem"
description: "Read properties and relationships of the listItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get listItem

Namespace: microsoft.graph

Read properties and relationships of the [listItem](../resources/listitem.md) object.

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
GET /shares/{sharesId}/listItem
GET /me/drive/list/items/{listItemId}
GET /workbooks/{workbooksId}/listItem
GET /me/drive/items/{driveItemId}/listItem
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/listItem
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
If successful, this method returns a `200 OK` response code and [listItem](../resources/listitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_listitem"
}
-->
``` http
GET https://graph.microsoft.com/localtest/shares/{sharesId}/listItem
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.listItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1625

{
  "value": {
    "@odata.type": "#microsoft.graph.listItem",
    "id": "a91474b4-74b4-a914-b474-14a9b47414a9",
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
    "webUrl": "https://example.com/webUrl/",
    "contentType": {
      "@odata.type": "microsoft.graph.contentTypeInfo"
    },
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds"
    }
  }
}
```

