---
title: "Update driveItemVersion"
description: "Update the properties of a driveItemVersion object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update driveItemVersion

Namespace: microsoft.graph

Update the properties of a [driveItemVersion](../resources/driveitemversion.md) object.

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
PATCH /workbooks/{workbooksId}/versions/{driveItemVersionId}
PATCH /me/drive/items/{driveItemId}/versions/{driveItemVersionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [driveItemVersion](../resources/driveitemversion.md) object.

The following table shows the properties that are required when you create the [driveItemVersion](../resources/driveitemversion.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|publication|[publicationFacet](../resources/publicationfacet.md)| Inherited from [baseItemVersion](../resources/baseitemversion.md)|
|content|Stream||
|size|Int64||



## Response
If successful, this method returns a `200 OK` response code and an updated [driveItemVersion](../resources/driveitemversion.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_driveitemversion"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/workbooks/{workbooksId}/versions/{driveItemVersionId}
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "Level value",
    "versionId": "Version Id value"
  },
  "content": "Stream",
  "size": 4
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
Content-Length: 730

{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "id": "a8f5016d-016d-a8f5-6d01-f5a86d01f5a8",
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
  },
  "content": "Stream",
  "size": 4
}
```

