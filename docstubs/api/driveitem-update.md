---
title: "Update driveItem"
description: "Update the properties of a driveItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update driveItem

Namespace: microsoft.graph

Update the properties of a [driveItem](../resources/driveitem.md) object.

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
PATCH /me/drive/root
PATCH /drives/{drivesId}/root
PATCH /shares/{sharesId}/root
PATCH /workbooks/{workbooksId}
PATCH /shares/{sharesId}/driveItem
PATCH /me/drive/items/{driveItemId}
PATCH /me/drive/special/{driveItemId}
PATCH /drives/{drivesId}/items/{driveItemId}
PATCH /shares/{sharesId}/items/{driveItemId}
PATCH /drives/{drivesId}/special/{driveItemId}
PATCH /workbooks/{workbooksId}/children/{driveItemId}
PATCH /me/drive/items/{driveItemId}/listItem/driveItem
PATCH /me/drive/items/{driveItemId}/children/{driveItemId}
PATCH /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/root
PATCH /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/driveItem
PATCH /me/joinedTeams/{groupId}/sites/{siteId}/items/{baseItemId}/microsoft.graph.sharedDriveItem/items/{driveItemId}
PATCH /me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/{itemActivityId}/driveItem
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [driveItem](../resources/driveitem.md) object.

The following table shows the properties that are required when you create the [driveItem](../resources/driveitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|description|String| Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|
|audio|[audio](../resources/audio.md)||
|content|Stream||
|cTag|String||
|deleted|[deleted](../resources/deleted.md)||
|file|[file](../resources/file.md)||
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)||
|folder|[folder](../resources/folder.md)||
|image|[image](../resources/image.md)||
|location|[geoCoordinates](../resources/geocoordinates.md)||
|package|[package](../resources/package.md)||
|photo|[photo](../resources/photo.md)||
|publication|[publicationFacet](../resources/publicationfacet.md)||
|remoteItem|[remoteItem](../resources/remoteitem.md)||
|root|[root](../resources/root.md)||
|searchResult|[searchResult](../resources/searchresult.md)||
|shared|[shared](../resources/shared.md)||
|sharepointIds|[sharepointIds](../resources/sharepointids.md)||
|size|Int64||
|specialFolder|[specialFolder](../resources/specialfolder.md)||
|video|[video](../resources/video.md)||
|webDavUrl|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [driveItem](../resources/driveitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_driveitem"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/root
Content-type: application/json
Content-length: 4666

{
  "@odata.type": "#microsoft.graph.driveItem",
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
  "webUrl": "https://example.com/webUrl/",
  "audio": {
    "@odata.type": "microsoft.graph.audio",
    "album": "Album value",
    "albumArtist": "Album Artist value",
    "artist": "Artist value",
    "bitrate": 7,
    "composers": "Composers value",
    "copyright": "Copyright value",
    "disc": 4,
    "discCount": 9,
    "duration": 8,
    "genre": "Genre value",
    "hasDrm": true,
    "isVariableBitrate": true,
    "title": "Title value",
    "track": 5,
    "trackCount": 10,
    "year": 4
  },
  "content": "Stream",
  "cTag": "CTag value",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted",
    "state": "State value"
  },
  "file": {
    "@odata.type": "microsoft.graph.file",
    "hashes": {
      "@odata.type": "microsoft.graph.hashes",
      "crc32Hash": "Crc32Hash value",
      "quickXorHash": "Quick Xor Hash value",
      "sha1Hash": "Sha1Hash value"
    },
    "mimeType": "Mime Type value",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "2017-01-01T00:01:01.6350302+03:00"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "childCount": 10,
    "view": {
      "@odata.type": "microsoft.graph.folderView",
      "sortBy": "Sort By value",
      "sortOrder": "Sort Order value",
      "viewType": "View Type value"
    }
  },
  "image": {
    "@odata.type": "microsoft.graph.image",
    "height": 6,
    "width": 5
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  },
  "package": {
    "@odata.type": "microsoft.graph.package",
    "type": "Type value"
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo",
    "cameraMake": "Camera Make value",
    "cameraModel": "Camera Model value",
    "exposureDenominator": "Double",
    "exposureNumerator": "Double",
    "fNumber": "Double",
    "focalLength": "Double",
    "iso": 3,
    "takenDateTime": "2016-12-31T23:58:02.7260171+03:00"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem",
    "shared": {
      "@odata.type": "microsoft.graph.shared",
      "owner": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "scope": "Scope value",
      "sharedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "sharedDateTime": "2017-01-01T00:03:31.2088126+03:00"
    },
    "size": 4,
    "specialFolder": {
      "@odata.type": "microsoft.graph.specialFolder"
    },
    "webDavUrl": "https://example.com/webDavUrl/"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult",
    "onClickTelemetryUrl": "https://example.com/onClickTelemetryUrl/"
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
    "@odata.type": "microsoft.graph.video",
    "audioBitsPerSample": 2,
    "audioChannels": 13,
    "audioFormat": "Audio Format value",
    "audioSamplesPerSecond": 5,
    "bitrate": 7,
    "fourCC": "Four CC value",
    "frameRate": "Double"
  },
  "webDavUrl": "https://example.com/webDavUrl/"
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
Content-Length: 4917

{
  "@odata.type": "#microsoft.graph.driveItem",
  "id": "32af1cdc-1cdc-32af-dc1c-af32dc1caf32",
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
  "audio": {
    "@odata.type": "microsoft.graph.audio",
    "album": "Album value",
    "albumArtist": "Album Artist value",
    "artist": "Artist value",
    "bitrate": 7,
    "composers": "Composers value",
    "copyright": "Copyright value",
    "disc": 4,
    "discCount": 9,
    "duration": 8,
    "genre": "Genre value",
    "hasDrm": true,
    "isVariableBitrate": true,
    "title": "Title value",
    "track": 5,
    "trackCount": 10,
    "year": 4
  },
  "content": "Stream",
  "cTag": "CTag value",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted",
    "state": "State value"
  },
  "file": {
    "@odata.type": "microsoft.graph.file",
    "hashes": {
      "@odata.type": "microsoft.graph.hashes",
      "crc32Hash": "Crc32Hash value",
      "quickXorHash": "Quick Xor Hash value",
      "sha1Hash": "Sha1Hash value"
    },
    "mimeType": "Mime Type value",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "2017-01-01T00:01:01.6350302+03:00"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "childCount": 10,
    "view": {
      "@odata.type": "microsoft.graph.folderView",
      "sortBy": "Sort By value",
      "sortOrder": "Sort Order value",
      "viewType": "View Type value"
    }
  },
  "image": {
    "@odata.type": "microsoft.graph.image",
    "height": 6,
    "width": 5
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  },
  "package": {
    "@odata.type": "microsoft.graph.package",
    "type": "Type value"
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo",
    "cameraMake": "Camera Make value",
    "cameraModel": "Camera Model value",
    "exposureDenominator": "Double",
    "exposureNumerator": "Double",
    "fNumber": "Double",
    "focalLength": "Double",
    "iso": 3,
    "takenDateTime": "2016-12-31T23:58:02.7260171+03:00"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem",
    "shared": {
      "@odata.type": "microsoft.graph.shared",
      "owner": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "scope": "Scope value",
      "sharedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "sharedDateTime": "2017-01-01T00:03:31.2088126+03:00"
    },
    "size": 4,
    "specialFolder": {
      "@odata.type": "microsoft.graph.specialFolder"
    },
    "webDavUrl": "https://example.com/webDavUrl/"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult",
    "onClickTelemetryUrl": "https://example.com/onClickTelemetryUrl/"
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
    "@odata.type": "microsoft.graph.video",
    "audioBitsPerSample": 2,
    "audioChannels": 13,
    "audioFormat": "Audio Format value",
    "audioSamplesPerSecond": 5,
    "bitrate": 7,
    "fourCC": "Four CC value",
    "frameRate": "Double"
  },
  "webDavUrl": "https://example.com/webDavUrl/"
}
```

