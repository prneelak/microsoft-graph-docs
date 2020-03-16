---
title: "List plans"
description: "Get the plannerPlans from the plans navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List plans

Namespace: microsoft.graph

Get the plannerPlans from the plans navigation property.

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
GET /me/joinedTeams/{groupId}/planner/plans
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
If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/planner/plans
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannerplan)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 692

{
  "value": [
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
  ]
}
```

