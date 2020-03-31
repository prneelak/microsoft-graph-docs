---
title: "List shared"
description: "Get the sharedInsights from the shared navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List shared

Namespace: microsoft.graph

Get the sharedInsights from the shared navigation property.

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
GET /me/insights/shared
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
If successful, this method returns a `200 OK` response code and a collection of [sharedInsight](../resources/sharedinsight.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sharedinsight"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/insights/shared
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sharedinsight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1494

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedInsight",
      "id": "23a21ce6-1ce6-23a2-e61c-a223e61ca223",
      "lastShared": {
        "@odata.type": "microsoft.graph.sharingDetail",
        "sharedBy": {
          "@odata.type": "microsoft.graph.insightIdentity",
          "displayName": "Display Name value",
          "id": "Id value",
          "address": "Address value"
        },
        "sharedDateTime": "2016-12-31T23:57:17.9322992+03:00",
        "sharingSubject": "Sharing Subject value",
        "sharingType": "Sharing Type value",
        "sharingReference": {
          "@odata.type": "microsoft.graph.resourceReference",
          "webUrl": "https://example.com/webUrl/",
          "type": "Type value"
        }
      },
      "sharingHistory": [
        {
          "@odata.type": "microsoft.graph.sharingDetail"
        }
      ],
      "resourceVisualization": {
        "@odata.type": "microsoft.graph.resourceVisualization",
        "title": "Title value",
        "mediaType": "Media Type value",
        "previewImageUrl": "https://example.com/previewImageUrl/",
        "previewText": "Preview Text value",
        "containerWebUrl": "https://example.com/containerWebUrl/",
        "containerDisplayName": "Container Display Name value",
        "containerType": "Container Type value"
      },
      "resourceReference": {
        "@odata.type": "microsoft.graph.resourceReference"
      }
    }
  ]
}
```

