---
title: "Add buckets"
description: "Add buckets by posting to the buckets collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add buckets

Namespace: microsoft.graph

Add buckets by posting to the buckets collection.

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
POST /planner/buckets/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [plannerBucket](../resources/plannerbucket.md) object.

The following table shows the properties that are required when you create the [plannerBucket](../resources/plannerbucket.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|planId|String||
|orderHint|String||



## Response
If successful, this method returns a `201 Created` response code and a [plannerBucket](../resources/plannerbucket.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/planner/buckets
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "name": "Name value",
  "planId": "Plan Id value",
  "orderHint": "Order Hint value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerbucket"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "id": "068b67c9-67c9-068b-c967-8b06c9678b06",
  "name": "Name value",
  "planId": "Plan Id value",
  "orderHint": "Order Hint value"
}
```

