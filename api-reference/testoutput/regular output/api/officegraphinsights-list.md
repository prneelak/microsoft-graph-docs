---
title: "List officeGraphInsightses"
description: "List properties and relationships of the officeGraphInsights objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List officeGraphInsightses

Namespace: microsoft.graph

List properties and relationships of the [officeGraphInsights](../resources/officegraphinsights.md) objects.

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
GET ** Collection URI for microsoft.graph.officeGraphInsights not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [officeGraphInsights](../resources/officegraphinsights.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_officegraphinsights"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.officeGraphInsights not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.officegraphinsights)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeGraphInsights",
      "id": "5ea118a8-18a8-5ea1-a818-a15ea818a15e"
    }
  ]
}
```

