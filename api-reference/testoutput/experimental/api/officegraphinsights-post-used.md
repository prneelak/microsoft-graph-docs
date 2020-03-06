---
title: "Add used"
description: "Add used by posting to the used collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add used

Namespace: microsoft.graph

Add used by posting to the used collection.

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
POST /me/insights/used/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [usedInsight](../resources/usedinsight.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_usedinsight_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/insights/used
Content-type: application/json
Content-length: 883

{
  "@odata.type": "#microsoft.graph.usedInsight",
  "lastUsed": {
    "@odata.type": "microsoft.graph.usageDetails",
    "lastAccessedDateTime": "2016-12-31T23:58:50.8669622+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
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
  "truncated": true,
  "@odata.type": "microsoft.graph.usedinsight"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 932

{
  "@odata.type": "#microsoft.graph.usedInsight",
  "id": "6b4978a5-78a5-6b49-a578-496ba578496b",
  "lastUsed": {
    "@odata.type": "microsoft.graph.usageDetails",
    "lastAccessedDateTime": "2016-12-31T23:58:50.8669622+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
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

