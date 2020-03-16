---
title: "Get trending"
description: "Read properties and relationships of the trending object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get trending

Namespace: microsoft.graph

Read properties and relationships of the [trending](../resources/trending.md) object.

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
GET /me/insights/trending/{trendingId}
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
If successful, this method returns a `200 OK` response code and [trending](../resources/trending.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_trending"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/insights/trending/{trendingId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trending"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 869

{
  "value": {
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
}
```

