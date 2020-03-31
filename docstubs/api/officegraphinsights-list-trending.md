---
title: "List trending"
description: "Get the trendings from the trending navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List trending

Namespace: microsoft.graph

Get the trendings from the trending navigation property.

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
GET /me/insights/trending
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [trending](../resources/trending.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_trending"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/insights/trending
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.trending)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 923

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.trending",
      "id": "3188765c-765c-3188-5c76-88315c768831",
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
      "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
    }
  ]
}
```

