---
title: "search"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# search

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
GET /me/drive/root/search
GET /drives/{drivesId}/root/search
GET /shares/{sharesId}/root/search
GET /workbooks/{workbooksId}/search
GET /shares/{sharesId}/driveItem/search
GET /me/drive/items/{driveItemId}/search
GET /me/drive/special/{driveItemId}/search
GET /drives/{drivesId}/items/{driveItemId}/search
GET /shares/{sharesId}/items/{driveItemId}/search
GET /drives/{drivesId}/special/{driveItemId}/search
GET /workbooks/{workbooksId}/children/{driveItemId}/search
GET /me/drive/items/{driveItemId}/listItem/driveItem/search
GET /me/drive/items/{driveItemId}/children/{driveItemId}/search
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root/search
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem/search
GET /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}/search
GET /me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem/search
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|q|String||



## Response
If successful, this function returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "driveitem_search"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/root/search(q='parameterValue')
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
Content-Length: 2224

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.driveItem",
      "id": "32af1cdc-1cdc-32af-dc1c-af32dc1caf32",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
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
        "@odata.type": "microsoft.graph.itemReference"
      },
      "webUrl": "https://example.com/webUrl/",
      "audio": {
        "@odata.type": "microsoft.graph.audio"
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

