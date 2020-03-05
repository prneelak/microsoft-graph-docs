---
title: "List operations"
description: "Get the teamsAsyncOperations from the operations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List operations

Namespace: microsoft.graph

Get the teamsAsyncOperations from the operations navigation property.

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
GET /teams/{teamsId}/operations
GET /me/joinedTeams/{groupId}/team/operations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsAsyncOperation](../resources/teamsasyncoperation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsasyncoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teams/{teamsId}/operations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsasyncoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsAsyncOperation",
      "id": "c0ad7dfc-7dfc-c0ad-fc7d-adc0fc7dadc0",
      "operationType": "String",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "status": "String",
      "lastActionDateTime": "2017-01-01T00:03:19.3737597+03:00",
      "attemptsCount": 13,
      "targetResourceId": "Target Resource Id value",
      "targetResourceLocation": "Target Resource Location value",
      "error": {
        "@odata.type": "microsoft.graph.operationError",
        "code": "Code value",
        "message": "Message value"
      }
    }
  ]
}
```

