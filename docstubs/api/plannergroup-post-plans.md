---
title: "Create plans"
description: "Create plans by posting to the plans collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create plans

Namespace: microsoft.graph

Create plans by posting to the plans collection.

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
POST /me/joinedTeams/{groupId}/planner/plans/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [plannerPlan](../resources/plannerplan.md) object.

The following table shows the properties that are required when you create the [plannerPlan](../resources/plannerplan.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset||
|owner|String||
|title|String||



## Response
If successful, this method returns a `201 Created` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/planner/plans
Content-type: application/json
Content-length: 475

{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "owner": "Owner value",
  "title": "Title value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerplan"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 583

{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "id": "bb5cb840-b840-bb5c-40b8-5cbb40b85cbb",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "owner": "Owner value",
  "title": "Title value"
}
```

