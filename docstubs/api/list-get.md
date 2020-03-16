---
title: "Get list"
description: "Read properties and relationships of the list object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get list

Namespace: microsoft.graph

Read properties and relationships of the [list](../resources/list.md) object.

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
GET /me/drive/list
GET /drives/{drivesId}/list
GET /shares/{sharesId}/list
GET /sites/{sitesId}/lists/{listId}
GET /me/joinedTeams/{groupId}/sites/{siteId}/lists/{listId}
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/list
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
If successful, this method returns a `200 OK` response code and [list](../resources/list.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_list"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/list
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.list"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1822

{
  "value": {
    "@odata.type": "#microsoft.graph.list",
    "id": "27b4ffc3-ffc3-27b4-c3ff-b427c3ffb427",
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
    "createdDateTime": "2017-01-01T00:03:06.9344969+03:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2016-12-31T23:59:32.0057525+03:00",
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
    "displayName": "Display Name value",
    "list": {
      "@odata.type": "microsoft.graph.listInfo",
      "contentTypesEnabled": true,
      "hidden": true,
      "template": "Template value"
    },
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds"
    },
    "system": {
      "@odata.type": "microsoft.graph.systemFacet"
    }
  }
}
```

