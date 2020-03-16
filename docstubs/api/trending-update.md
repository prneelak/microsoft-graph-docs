---
title: "Update trending"
description: "Update the properties of a trending object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update trending

Namespace: microsoft.graph

Update the properties of a [trending](../resources/trending.md) object.

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
PATCH /me/insights/trending/{trendingId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [trending](../resources/trending.md) object.

The following table shows the properties that are required when you create the [trending](../resources/trending.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|weight|Double||
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)||
|resourceReference|[resourceReference](../resources/resourcereference.md)||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [trending](../resources/trending.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_trending"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/insights/trending/{trendingId}
Content-type: application/json
Content-length: 697

{
  "@odata.type": "#microsoft.graph.trending",
  "weight": "Double",
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization",
    "title": "Title value",
    "type": "Type value",
    "mediaType": "Media Type value",
    "previewImageUrl": "https://example.com/previewImageUrl/",
    "previewText": "Preview Text value",
    "containerWebUrl": "https://example.com/containerWebUrl/",
    "containerDisplayName": "Container Display Name value",
    "containerType": "Container Type value"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference",
    "webUrl": "https://example.com/webUrl/",
    "id": "Id value"
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
Content-Length: 810

{
  "@odata.type": "#microsoft.graph.trending",
  "id": "b66a214e-214e-b66a-4e21-6ab64e216ab6",
  "weight": "Double",
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization",
    "title": "Title value",
    "type": "Type value",
    "mediaType": "Media Type value",
    "previewImageUrl": "https://example.com/previewImageUrl/",
    "previewText": "Preview Text value",
    "containerWebUrl": "https://example.com/containerWebUrl/",
    "containerDisplayName": "Container Display Name value",
    "containerType": "Container Type value"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference",
    "webUrl": "https://example.com/webUrl/",
    "id": "Id value"
  },
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00"
}
```

