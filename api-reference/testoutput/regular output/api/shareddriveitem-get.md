---
title: "Get sharedDriveItem"
description: "Read properties and relationships of the sharedDriveItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get sharedDriveItem

Namespace: microsoft.graph

Read properties and relationships of the [sharedDriveItem](../resources/shareddriveitem.md) object.

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
GET /shares/{sharesId}
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
If successful, this method returns a `200 OK` response code and [sharedDriveItem](../resources/shareddriveitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_shareddriveitem"
}
-->
``` http
GET https://graph.microsoft.com/localtest/shares/{sharesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedDriveItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1536

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedDriveItem",
    "id": "f28e5cbd-5cbd-f28e-bd5c-8ef2bd5c8ef2",
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
    "createdDateTime": "2016-12-31T23:57:43.7581228+03:00",
    "description": "Description value",
    "eTag": "ETag value",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2017-01-01T00:00:06.8007887+03:00",
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
    "owner": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

