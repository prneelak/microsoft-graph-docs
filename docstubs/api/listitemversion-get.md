---
title: "Get listItemVersion"
description: "Read properties and relationships of the listItemVersion object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get listItemVersion

Namespace: microsoft.graph

Read properties and relationships of the [listItemVersion](../resources/listitemversion.md) object.

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
GET /me/drive/items/{driveItemId}/listItem/versions/{listItemVersionId}
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
If successful, this method returns a `200 OK` response code and [listItemVersion](../resources/listitemversion.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_listitemversion"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/listItem/versions/{listItemVersionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.listItemVersion"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 754

{
  "value": {
    "@odata.type": "#microsoft.graph.listItemVersion",
    "id": "f80f6c3d-6c3d-f80f-3d6c-0ff83d6c0ff8",
    "lastModifiedBy": {
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
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
    "publication": {
      "@odata.type": "microsoft.graph.publicationFacet",
      "level": "Level value",
      "versionId": "Version Id value"
    }
  }
}
```

