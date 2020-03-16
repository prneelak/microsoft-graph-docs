---
title: "List used"
description: "Get the usedInsights from the used navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List used

Namespace: microsoft.graph

Get the usedInsights from the used navigation property.

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
GET /me/insights/used
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
If successful, this method returns a `200 OK` response code and a collection of [usedInsight](../resources/usedinsight.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usedinsight"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/insights/used
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.usedinsight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1057

{
  "value": [
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
  ]
}
```

