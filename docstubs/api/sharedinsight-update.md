---
title: "Update sharedInsight"
description: "Update the properties of a sharedInsight object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sharedInsight

Namespace: microsoft.graph

Update the properties of a [sharedInsight](../resources/sharedinsight.md) object.

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
PATCH /me/insights/shared/{sharedInsightId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [sharedInsight](../resources/sharedinsight.md) object.

The following table shows the properties that are required when you create the [sharedInsight](../resources/sharedinsight.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastShared|[sharingDetail](../resources/sharingdetail.md)||
|sharingHistory|[sharingDetail](../resources/sharingdetail.md) collection||
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)||
|resourceReference|[resourceReference](../resources/resourcereference.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [sharedInsight](../resources/sharedinsight.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sharedinsight"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/insights/shared/{sharedInsightId}
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail",
    "sharedBy": {
      "@odata.type": "microsoft.graph.insightIdentity",
      "displayName": "Display Name value",
      "id": "Id value",
      "address": "Address value"
    },
    "sharedDateTime": "2017-01-01T00:03:31.2088126+03:00",
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
Content-Length: 1313

{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "id": "4958acb6-acb6-4958-b6ac-5849b6ac5849",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail",
    "sharedBy": {
      "@odata.type": "microsoft.graph.insightIdentity",
      "displayName": "Display Name value",
      "id": "Id value",
      "address": "Address value"
    },
    "sharedDateTime": "2017-01-01T00:03:31.2088126+03:00",
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
```

