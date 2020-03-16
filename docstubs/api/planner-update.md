---
title: "Update planner"
description: "Update the properties of a planner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update planner

Namespace: microsoft.graph

Update the properties of a [planner](../resources/planner.md) object.

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
PATCH /planner
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [planner](../resources/planner.md) object.

The following table shows the properties that are required when you create the [planner](../resources/planner.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [planner](../resources/planner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_planner"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/planner
Content-type: application/json
Content-length: 49

{
  "@odata.type": "#microsoft.graph.planner"
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
Content-Length: 98

{
  "@odata.type": "#microsoft.graph.planner",
  "id": "22a8aa69-aa69-22a8-69aa-a82269aaa822"
}
```

