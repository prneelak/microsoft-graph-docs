---
title: "Get driveItem"
description: "Read the properties and relationships of a driveItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get driveItem

Namespace: microsoft.graph

Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /workbooks/{workbooksId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_driveitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.driveItem",
    "id": "9a00594e-594e-9a00-4e59-009a4e59009a",
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
      "@odata.type": "microsoft.graph.itemReference"
    },
    "webUrl": "String",
    "audio": {
      "@odata.type": "microsoft.graph.audio"
    },
    "bundle": {
      "@odata.type": "microsoft.graph.bundle"
    },
    "content": "Stream",
    "cTag": "String",
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
    "size": "Integer",
    "specialFolder": {
      "@odata.type": "microsoft.graph.specialFolder"
    },
    "video": {
      "@odata.type": "microsoft.graph.video"
    },
    "webDavUrl": "String"
  }
}
```

