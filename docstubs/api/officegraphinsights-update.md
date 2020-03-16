---
title: "Update officeGraphInsights"
description: "Update the properties of a officeGraphInsights object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update officeGraphInsights

Namespace: microsoft.graph

Update the properties of a [officeGraphInsights](../resources/officegraphinsights.md) object.

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
PATCH /me/insights
PATCH /users/{usersId}/insights
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [officeGraphInsights](../resources/officegraphinsights.md) object.

The following table shows the properties that are required when you create the [officeGraphInsights](../resources/officegraphinsights.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [officeGraphInsights](../resources/officegraphinsights.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_officegraphinsights"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/insights
Content-type: application/json
Content-length: 61

{
  "@odata.type": "#microsoft.graph.officeGraphInsights"
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
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.officeGraphInsights",
  "id": "8a5236b1-36b1-8a52-b136-528ab136528a"
}
```

