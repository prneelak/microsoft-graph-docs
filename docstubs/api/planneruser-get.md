---
title: "Get plannerUser"
description: "Read properties and relationships of the plannerUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get plannerUser

Namespace: microsoft.graph

Read properties and relationships of the [plannerUser](../resources/planneruser.md) object.

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
GET /me/planner
GET /users/{usersId}/planner
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
If successful, this method returns a `200 OK` response code and [plannerUser](../resources/planneruser.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_planneruser"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/planner
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 361

{
  "value": {
    "@odata.type": "#microsoft.graph.plannerUser",
    "id": "5c6c83c7-83c7-5c6c-c783-6c5cc7836c5c",
    "favoritePlanReferences": {
      "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
    },
    "recentPlanReferences": {
      "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
    }
  }
}
```

