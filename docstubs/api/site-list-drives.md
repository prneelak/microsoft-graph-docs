---
title: "List drives"
description: "Get the drives from the drives navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List drives

Namespace: microsoft.graph

Get the drives from the drives navigation property.

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
GET /sites/{sitesId}/drives
GET /me/joinedTeams/{groupId}/sites/{siteId}/drives
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
If successful, this method returns a `200 OK` response code and a collection of [drive](../resources/drive.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_drive"
}
-->
``` http
GET https://graph.microsoft.com/localtest/sites/{sitesId}/drives
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.drive)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2041

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.drive",
      "id": "c9b50061-0061-c9b5-6100-b5c96100b5c9",
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
      "createdDateTime": "2017-01-01T00:00:51.2796212+03:00",
      "description": "Description value",
      "eTag": "ETag value",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "2016-12-31T23:57:58.0056135+03:00",
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
  ]
}
```

