---
title: "Update usedInsight"
description: "Update the properties of a usedInsight object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update usedInsight

Namespace: microsoft.graph

Update the properties of a [usedInsight](../resources/usedinsight.md) object.

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
PATCH /me/insights/used/{usedInsightId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [usedInsight](../resources/usedinsight.md) object.

The following table shows the properties that are required when you create the [usedInsight](../resources/usedinsight.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUsed|[usageDetails](../resources/usagedetails.md)||
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)||
|resourceReference|[resourceReference](../resources/resourcereference.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [usedInsight](../resources/usedinsight.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_usedinsight"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/insights/used/{usedInsightId}
Content-type: application/json
Content-length: 883

{
  "@odata.type": "#microsoft.graph.usedInsight",
  "lastUsed": {
    "@odata.type": "microsoft.graph.usageDetails",
    "lastAccessedDateTime": "2017-01-01T00:01:01.6350302+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00"
  },
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
Content-Length: 932

{
  "@odata.type": "#microsoft.graph.usedInsight",
  "id": "99be1c5e-1c5e-99be-5e1c-be995e1cbe99",
  "lastUsed": {
    "@odata.type": "microsoft.graph.usageDetails",
    "lastAccessedDateTime": "2017-01-01T00:01:01.6350302+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00"
  },
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

