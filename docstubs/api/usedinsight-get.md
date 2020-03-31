---
title: "Get usedInsight"
description: "Read properties and relationships of the usedInsight object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get usedInsight

Namespace: microsoft.graph

Read properties and relationships of the [usedInsight](../resources/usedinsight.md) object.

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
GET /me/insights/used/{usedInsightId}
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
If successful, this method returns a `200 OK` response code and [usedInsight](../resources/usedinsight.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usedinsight"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/insights/used/{usedInsightId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 997

{
  "value": {
    "@odata.type": "#microsoft.graph.usedInsight",
    "id": "0cf237db-37db-0cf2-db37-f20cdb37f20c",
    "lastUsed": {
      "@odata.type": "microsoft.graph.usageDetails",
      "lastAccessedDateTime": "2016-12-31T23:59:14.3499032+03:00",
      "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00"
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
}
```

