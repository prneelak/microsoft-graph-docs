---
title: "Update plannerUser"
description: "Update the properties of a plannerUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerUser

Namespace: microsoft.graph

Update the properties of a [plannerUser](../resources/planneruser.md) object.

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
PATCH /me/planner
PATCH /users/{usersId}/planner
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerUser](../resources/planneruser.md) object.

The following table shows the properties that are required when you create the [plannerUser](../resources/planneruser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)||
|recentPlanReferences|[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerUser](../resources/planneruser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_planneruser"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/planner
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.plannerUser",
  "favoritePlanReferences": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
  },
  "recentPlanReferences": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
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
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.plannerUser",
  "id": "b04d1a29-1a29-b04d-291a-4db0291a4db0",
  "favoritePlanReferences": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
  },
  "recentPlanReferences": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
  }
}
```

