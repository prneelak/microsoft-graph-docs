---
title: "Update plannerProgressTaskBoardTaskFormat"
description: "Update the properties of a plannerProgressTaskBoardTaskFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerProgressTaskBoardTaskFormat

Namespace: microsoft.graph

Update the properties of a [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.

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
PATCH /me/planner/tasks/{plannerTaskId}/progressTaskBoardFormat
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.

The following table shows the properties that are required when you create the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHint|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/planner/tasks/{plannerTaskId}/progressTaskBoardFormat
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "orderHint": "Order Hint value"
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
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "id": "8f7ddb20-db20-8f7d-20db-7d8f20db7d8f",
  "orderHint": "Order Hint value"
}
```

