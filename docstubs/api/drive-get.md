---
title: "Get drive"
description: "Read properties and relationships of the drive object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get drive

Namespace: microsoft.graph

Read properties and relationships of the [drive](../resources/drive.md) object.

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
GET /drive
GET /me/drive
GET /drives/{drivesId}
GET /me/drive/list/drive
GET /me/drives/{driveId}
GET /users/{usersId}/drive
GET /sites/{sitesId}/drive
GET /groups/{groupsId}/drive
GET /me/joinedTeams/{groupId}/drive
GET /users/{usersId}/drives/{driveId}
GET /sites/{sitesId}/drives/{driveId}
GET /groups/{groupsId}/drives/{driveId}
GET /me/joinedTeams/{groupId}/drives/{driveId}
GET /me/joinedTeams/{groupId}/sites/{siteId}/drive
GET /me/joinedTeams/{groupId}/sites/{siteId}/drives/{driveId}
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
If successful, this method returns a `200 OK` response code and [drive](../resources/drive.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_drive"
}
-->
``` http
GET https://graph.microsoft.com/localtest/drive
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1909

{
  "value": {
    "@odata.type": "#microsoft.graph.drive",
    "id": "98509293-9293-9850-9392-509893925098",
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
    "createdDateTime": "2016-12-31T23:56:44.0896282+03:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2017-01-01T00:01:48.4379164+03:00",
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
    "driveType": "Drive Type value",
    "owner": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "quota": {
      "@odata.type": "microsoft.graph.quota",
      "deleted": 7,
      "remaining": 9,
      "state": "State value",
      "total": 5,
      "used": 4
    },
    "sharePointIds": {
      "@odata.type": "microsoft.graph.sharepointIds"
    },
    "system": {
      "@odata.type": "microsoft.graph.systemFacet"
    }
  }
}
```

