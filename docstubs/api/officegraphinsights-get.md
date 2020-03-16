---
title: "Get officeGraphInsights"
description: "Read properties and relationships of the officeGraphInsights object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get officeGraphInsights

Namespace: microsoft.graph

Read properties and relationships of the [officeGraphInsights](../resources/officegraphinsights.md) object.

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
GET /me/insights
GET /users/{usersId}/insights
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
If successful, this method returns a `200 OK` response code and [officeGraphInsights](../resources/officegraphinsights.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_officegraphinsights"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/insights
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officeGraphInsights"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.officeGraphInsights",
    "id": "8a5236b1-36b1-8a52-b136-528ab136528a"
  }
}
```

