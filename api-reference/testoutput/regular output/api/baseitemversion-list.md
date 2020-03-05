---
title: "List baseItemVersions"
description: "List properties and relationships of the baseItemVersion objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List baseItemVersions

Namespace: microsoft.graph

List properties and relationships of the [baseItemVersion](../resources/baseitemversion.md) objects.

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
GET ** Collection URI for microsoft.graph.baseItemVersion not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [baseItemVersion](../resources/baseitemversion.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_baseitemversion"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.baseItemVersion not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.baseitemversion)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.baseItemVersion",
      "id": "e397a058-a058-e397-58a0-97e358a097e3",
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
      }
    }
  ]
}
```

