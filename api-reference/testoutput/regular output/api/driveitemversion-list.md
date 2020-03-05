---
title: "List driveItemVersions"
description: "List properties and relationships of the driveItemVersion objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List driveItemVersions

Namespace: microsoft.graph

List properties and relationships of the [driveItemVersion](../resources/driveitemversion.md) objects.

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
GET /workbooks/{workbooksId}/versions
GET /me/drive/items/{driveItemId}/versions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [driveItemVersion](../resources/driveitemversion.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_driveitemversion"
}
-->
``` http
GET https://graph.microsoft.com/localtest/workbooks/{workbooksId}/versions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.driveitemversion)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 857

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.driveItemVersion",
      "id": "875bb8b5-b8b5-875b-b5b8-5b87b5b85b87",
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
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "publication": {
        "@odata.type": "microsoft.graph.publicationFacet",
        "level": "Level value",
        "versionId": "Version Id value"
      },
      "content": "Stream",
      "size": 4
    }
  ]
}
```

