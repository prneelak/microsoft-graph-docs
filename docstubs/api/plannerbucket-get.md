---
title: "Get plannerBucket"
description: "Read properties and relationships of the plannerBucket object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get plannerBucket

Namespace: microsoft.graph

Read properties and relationships of the [plannerBucket](../resources/plannerbucket.md) object.

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
GET /planner/buckets/{plannerBucketId}
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
If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/buckets/{plannerBucketId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 224

{
  "value": {
    "@odata.type": "#microsoft.graph.plannerBucket",
    "id": "cfad9892-9892-cfad-9298-adcf9298adcf",
    "name": "Name value",
    "planId": "Plan Id value",
    "orderHint": "Order Hint value"
  }
}
```

