---
title: "recent"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# recent

Namespace: microsoft.graph



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
GET /drive/recent
GET /me/drive/recent
GET /drives/{drivesId}/recent
GET /me/drives/{driveId}/recent
GET /users/{usersId}/drive/recent
GET /sites/{sitesId}/drive/recent
GET /groups/{groupsId}/drive/recent
GET /me/joinedGroups/{groupId}/drive/recent
GET /users/{usersId}/drives/{driveId}/recent
GET /sites/{sitesId}/drives/{driveId}/recent
GET /groups/{groupsId}/drives/{driveId}/recent
GET /me/joinedGroups/{groupId}/drive/list/drive/recent
GET /me/joinedGroups/{groupId}/drives/{driveId}/recent
GET /me/joinedGroups/{groupId}/sites/{siteId}/drive/recent
GET /me/joinedGroups/{groupId}/sites/{siteId}/drives/{driveId}/recent
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "drive_recent"
}
-->
``` http
GET https://graph.microsoft.com/beta/drive/recent
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.driveitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2402

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.driveItem",
      "id": "540bcfac-cfac-540b-accf-0b54accf0b54",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
      "name": "Name value",
      "parentReference": {
        "@odata.type": "microsoft.graph.itemReference"
      },
      "webUrl": "https://example.com/webUrl/",
      "audio": {
        "@odata.type": "microsoft.graph.audio"
      },
      "bundle": {
        "@odata.type": "microsoft.graph.bundle"
      },
      "content": "Stream",
      "cTag": "CTag value",
      "deleted": {
        "@odata.type": "microsoft.graph.deleted"
      },
      "file": {
        "@odata.type": "microsoft.graph.file"
      },
      "fileSystemInfo": {
        "@odata.type": "microsoft.graph.fileSystemInfo"
      },
      "folder": {
        "@odata.type": "microsoft.graph.folder"
      },
      "image": {
        "@odata.type": "microsoft.graph.image"
      },
      "location": {
        "@odata.type": "microsoft.graph.geoCoordinates"
      },
      "package": {
        "@odata.type": "microsoft.graph.package"
      },
      "pendingOperations": {
        "@odata.type": "microsoft.graph.pendingOperations"
      },
      "photo": {
        "@odata.type": "microsoft.graph.photo"
      },
      "publication": {
        "@odata.type": "microsoft.graph.publicationFacet"
      },
      "remoteItem": {
        "@odata.type": "microsoft.graph.remoteItem"
      },
      "root": {
        "@odata.type": "microsoft.graph.root"
      },
      "searchResult": {
        "@odata.type": "microsoft.graph.searchResult"
      },
      "shared": {
        "@odata.type": "microsoft.graph.shared"
      },
      "sharepointIds": {
        "@odata.type": "microsoft.graph.sharepointIds"
      },
      "size": 4,
      "specialFolder": {
        "@odata.type": "microsoft.graph.specialFolder"
      },
      "video": {
        "@odata.type": "microsoft.graph.video"
      },
      "webDavUrl": "https://example.com/webDavUrl/"
    }
  ]
}
```

