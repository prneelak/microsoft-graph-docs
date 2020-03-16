---
title: "Add versions"
description: "Add versions by posting to the versions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add versions

Namespace: microsoft.graph

Add versions by posting to the versions collection.

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
POST /me/drive/items/{driveItemId}/listItem/versions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [listItemVersion](../resources/listitemversion.md) object.

The following table shows the properties that are required when you create the [listItemVersion](../resources/listitemversion.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|



## Response
If successful, this method returns a `201 Created` response code and a [listItemVersion](../resources/listitemversion.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_listitemversion_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/listItem/versions
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.listItemVersion",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.listitemversion"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 691

{
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
```

