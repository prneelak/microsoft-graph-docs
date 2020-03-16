---
title: "Update thumbnailSet"
description: "Update the properties of a thumbnailSet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update thumbnailSet

Namespace: microsoft.graph

Update the properties of a [thumbnailSet](../resources/thumbnailset.md) object.

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
PATCH /workbooks/{workbooksId}/thumbnails/{thumbnailSetId}
PATCH /me/drive/items/{driveItemId}/thumbnails/{thumbnailSetId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [thumbnailSet](../resources/thumbnailset.md) object.

The following table shows the properties that are required when you create the [thumbnailSet](../resources/thumbnailset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|large|[thumbnail](../resources/thumbnail.md)||
|medium|[thumbnail](../resources/thumbnail.md)||
|small|[thumbnail](../resources/thumbnail.md)||
|source|[thumbnail](../resources/thumbnail.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [thumbnailSet](../resources/thumbnailset.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_thumbnailset"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/workbooks/{workbooksId}/thumbnails/{thumbnailSetId}
Content-type: application/json
Content-length: 459

{
  "@odata.type": "#microsoft.graph.thumbnailSet",
  "large": {
    "@odata.type": "microsoft.graph.thumbnail",
    "content": "Stream",
    "height": 6,
    "sourceItemId": "Source Item Id value",
    "url": "Url value",
    "width": 5
  },
  "medium": {
    "@odata.type": "microsoft.graph.thumbnail"
  },
  "small": {
    "@odata.type": "microsoft.graph.thumbnail"
  },
  "source": {
    "@odata.type": "microsoft.graph.thumbnail"
  }
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
Content-Length: 508

{
  "@odata.type": "#microsoft.graph.thumbnailSet",
  "id": "ec4febac-ebac-ec4f-aceb-4fecaceb4fec",
  "large": {
    "@odata.type": "microsoft.graph.thumbnail",
    "content": "Stream",
    "height": 6,
    "sourceItemId": "Source Item Id value",
    "url": "Url value",
    "width": 5
  },
  "medium": {
    "@odata.type": "microsoft.graph.thumbnail"
  },
  "small": {
    "@odata.type": "microsoft.graph.thumbnail"
  },
  "source": {
    "@odata.type": "microsoft.graph.thumbnail"
  }
}
```

