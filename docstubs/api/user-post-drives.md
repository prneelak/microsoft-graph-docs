---
title: "Add drives"
description: "Add drives by posting to the drives collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add drives

Namespace: microsoft.graph

Add drives by posting to the drives collection.

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
POST /me/drives/$ref
POST /users/{usersId}/drives/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [drive](../resources/drive.md) object.

The following table shows the properties that are required when you create the [drive](../resources/drive.md).

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
|driveType|String||
|owner|[identitySet](../resources/identityset.md)||
|quota|[quota](../resources/quota.md)||
|sharePointIds|[sharepointIds](../resources/sharepointids.md)||
|system|[systemFacet](../resources/systemfacet.md)||



## Response
If successful, this method returns a `201 Created` response code and a [drive](../resources/drive.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_drive_from_drives"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drives
Content-type: application/json
Content-length: 1521

{
  "@odata.type": "#microsoft.graph.drive",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1772

{
  "@odata.type": "#microsoft.graph.drive",
  "id": "3431ce90-ce90-3431-90ce-313490ce3134",
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
```

