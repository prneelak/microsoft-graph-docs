---
title: "Update plannerAssignedToTaskBoardTaskFormat"
description: "Update the properties of a plannerAssignedToTaskBoardTaskFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerAssignedToTaskBoardTaskFormat

Namespace: microsoft.graph

Update the properties of a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.

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
PATCH /me/planner/tasks/{plannerTaskId}/assignedToTaskBoardFormat
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.

The following table shows the properties that are required when you create the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|unassignedOrderHint|String||
|orderHintsByAssignee|[plannerOrderHintsByAssignee](../resources/plannerorderhintsbyassignee.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/planner/tasks/{plannerTaskId}/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "unassignedOrderHint": "Unassigned Order Hint value",
  "orderHintsByAssignee": {
    "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
  }
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
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "id": "b3c6cf17-cf17-b3c6-17cf-c6b317cfc6b3",
  "unassignedOrderHint": "Unassigned Order Hint value",
  "orderHintsByAssignee": {
    "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
  }
}
```

