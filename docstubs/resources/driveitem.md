---
title: "driveItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# driveItem resource type


Namespace: microsoft.graph




Inherits from [baseItem](../resources/baseitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List driveItems](../api/driveitem-list.md)|[driveItem](../resources/driveitem.md) collection|List properties and relationships of the [driveItem](../resources/driveitem.md) objects.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[Create driveItem](../api/driveitem-post-workbooks.md)|[driveItem](../resources/driveitem.md)|Create a new [driveItem](../resources/driveitem.md) object.|
|[Delete driveItem](../api/driveitem-delete.md)|None|Deletes a [driveItem](../resources/driveitem.md).|
|[Update driveItem](../api/driveitem-update.md)|[driveItem](../resources/driveitem.md)|Update the properties of a [driveItem](../resources/driveitem.md) object.|
|[delta](../api/driveitem-delta.md)|[driveItem](../resources/driveitem.md) collection||
|[delta](../api/driveitem-delta.md)|[driveItem](../resources/driveitem.md) collection||
|[getActivitiesByInterval](../api/driveitem-getactivitiesbyinterval.md)|[itemActivityStat](../resources/itemactivitystat.md) collection||
|[search](../api/driveitem-search.md)|[driveItem](../resources/driveitem.md) collection||
|[checkin](../api/driveitem-checkin.md)|None||
|[checkout](../api/driveitem-checkout.md)|None||
|[copy](../api/driveitem-copy.md)|[driveItem](../resources/driveitem.md)||
|[createLink](../api/driveitem-createlink.md)|[permission](../resources/permission.md)||
|[createUploadSession](../api/driveitem-createuploadsession.md)|[uploadSession](../resources/uploadsession.md)||
|[invite](../api/driveitem-invite.md)|[permission](../resources/permission.md) collection||
|[preview](../api/driveitem-preview.md)|[itemPreviewInfo](../resources/itempreviewinfo.md)||
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|
|[Get workbook](../api/workbook-get.md)|[workbook](../resources/workbook.md)|Read properties and relationships of the [workbook](../resources/workbook.md) object.|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemanalytics.md)|Read properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) object.|
|[List children](../api/driveitem-list-children.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the children navigation property.|
|[Add children](../api/driveitem-post-children.md)|[driveItem](../resources/driveitem.md)|Add children by posting to the children collection.|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listitem.md)|Read properties and relationships of the [listItem](../resources/listitem.md) object.|
|[List permissions](../api/driveitem-list-permissions.md)|[permission](../resources/permission.md) collection|Get the permissions from the permissions navigation property.|
|[Add permissions](../api/driveitem-post-permissions.md)|[permission](../resources/permission.md)|Add permissions by posting to the permissions collection.|
|[List subscriptions](../api/driveitem-list-subscriptions.md)|[subscription](../resources/subscription.md) collection|Get the subscriptions from the subscriptions navigation property.|
|[Add subscriptions](../api/driveitem-post-subscriptions.md)|[subscription](../resources/subscription.md)|Add subscriptions by posting to the subscriptions collection.|
|[List thumbnails](../api/driveitem-list-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md) collection|Get the thumbnailSets from the thumbnails navigation property.|
|[Add thumbnails](../api/driveitem-post-thumbnails.md)|[thumbnailSet](../resources/thumbnailset.md)|Add thumbnails by posting to the thumbnails collection.|
|[List versions](../api/driveitem-list-versions.md)|[driveItemVersion](../resources/driveitemversion.md) collection|Get the driveItemVersions from the versions navigation property.|
|[Add versions](../api/driveitem-post-versions.md)|[driveItemVersion](../resources/driveitemversion.md)|Add versions by posting to the versions collection.|
|[List children](../api/driveitem-list-children.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the children navigation property.|
|[Add children](../api/driveitem-post-children.md)|[driveItem](../resources/driveitem.md)|Add children by posting to the children collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|audio|[audio](../resources/audio.md)||
|content|Stream||
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|cTag|String||
|deleted|[deleted](../resources/deleted.md)||
|description|String| Inherited from [baseItem](../resources/baseitem.md)|
|eTag|String| Inherited from [baseItem](../resources/baseitem.md)|
|file|[file](../resources/file.md)||
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)||
|folder|[folder](../resources/folder.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|image|[image](../resources/image.md)||
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItem](../resources/baseitem.md)|
|location|[geoCoordinates](../resources/geocoordinates.md)||
|name|String| Inherited from [baseItem](../resources/baseitem.md)|
|package|[package](../resources/package.md)||
|parentReference|[itemReference](../resources/itemreference.md)| Inherited from [baseItem](../resources/baseitem.md)|
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
|webUrl|String| Inherited from [baseItem](../resources/baseitem.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|analytics|[itemAnalytics](../resources/itemanalytics.md)||
|children|[driveItem](../resources/driveitem.md) collection||
|createdByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|lastModifiedByUser|[user](../resources/user.md)| Inherited from [baseItem](../resources/baseitem.md)|
|listItem|[listItem](../resources/listitem.md)||
|permissions|[permission](../resources/permission.md) collection||
|subscriptions|[subscription](../resources/subscription.md) collection||
|thumbnails|[thumbnailSet](../resources/thumbnailset.md) collection||
|versions|[driveItemVersion](../resources/driveitemversion.md) collection||
|workbook|[workbook](../resources/workbook.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItem",
  "baseType": "microsoft.graph.baseItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.driveItem",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference",
    "driveId": "String",
    "driveType": "String",
    "path": "String",
    "shareId": "String",
    "sharepointIds": {
      "@odata.type": "microsoft.graph.sharepointIds",
      "listId": "String",
      "listItemId": "String",
      "listItemUniqueId": "String",
      "siteId": "String",
      "siteUrl": "String",
      "webId": "String"
    }
  },
  "webUrl": "String",
  "audio": {
    "@odata.type": "microsoft.graph.audio",
    "album": "String",
    "albumArtist": "String",
    "artist": "String",
    "bitrate": 1024,
    "composers": "String",
    "copyright": "String",
    "disc": 1024,
    "discCount": 1024,
    "duration": 1024,
    "genre": "String",
    "hasDrm": true,
    "isVariableBitrate": true,
    "title": "String",
    "track": 1024,
    "trackCount": 1024,
    "year": 1024
  },
  "content": "Stream",
  "cTag": "String",
  "deleted": {
    "@odata.type": "microsoft.graph.deleted",
    "state": "String"
  },
  "file": {
    "@odata.type": "microsoft.graph.file",
    "hashes": {
      "@odata.type": "microsoft.graph.hashes",
      "crc32Hash": "String",
      "quickXorHash": "String",
      "sha1Hash": "String"
    },
    "mimeType": "String",
    "processingMetadata": true
  },
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "lastAccessedDateTime": "String (timestamp)"
  },
  "folder": {
    "@odata.type": "microsoft.graph.folder",
    "childCount": 1024,
    "view": {
      "@odata.type": "microsoft.graph.folderView",
      "sortBy": "String",
      "sortOrder": "String",
      "viewType": "String"
    }
  },
  "image": {
    "@odata.type": "microsoft.graph.image",
    "height": 1024,
    "width": 1024
  },
  "location": {
    "@odata.type": "microsoft.graph.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  },
  "package": {
    "@odata.type": "microsoft.graph.package",
    "type": "String"
  },
  "photo": {
    "@odata.type": "microsoft.graph.photo",
    "cameraMake": "String",
    "cameraModel": "String",
    "exposureDenominator": "Double",
    "exposureNumerator": "Double",
    "fNumber": "Double",
    "focalLength": "Double",
    "iso": 1024,
    "takenDateTime": "String (timestamp)"
  },
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "remoteItem": {
    "@odata.type": "microsoft.graph.remoteItem",
    "shared": {
      "@odata.type": "microsoft.graph.shared",
      "owner": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "scope": "String",
      "sharedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "sharedDateTime": "String (timestamp)"
    },
    "specialFolder": {
      "@odata.type": "microsoft.graph.specialFolder"
    },
    "webDavUrl": "String"
  },
  "root": {
    "@odata.type": "microsoft.graph.root"
  },
  "searchResult": {
    "@odata.type": "microsoft.graph.searchResult",
    "onClickTelemetryUrl": "String"
  },
  "shared": {
    "@odata.type": "microsoft.graph.shared"
  },
  "sharepointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "size": 1024,
  "specialFolder": {
    "@odata.type": "microsoft.graph.specialFolder"
  },
  "video": {
    "@odata.type": "microsoft.graph.video",
    "audioBitsPerSample": 1024,
    "audioChannels": 1024,
    "audioFormat": "String",
    "audioSamplesPerSecond": 1024,
    "bitrate": 1024,
    "fourCC": "String",
    "frameRate": "Double"
  },
  "webDavUrl": "String"
}
```

