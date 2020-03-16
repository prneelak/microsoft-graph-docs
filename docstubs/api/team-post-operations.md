---
title: "Add operations"
description: "Add operations by posting to the operations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add operations

Namespace: microsoft.graph

Add operations by posting to the operations collection.

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
POST /teams/{teamsId}/operations/$ref
POST /me/joinedTeams/{groupId}/team/operations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.

The following table shows the properties that are required when you create the [teamsAsyncOperation](../resources/teamsasyncoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|operationType|Enumeration|. Possible values are: `invalid`, `cloneTeam`, `archiveTeam`, `unarchiveTeam`, `createTeam`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `invalid`, `notStarted`, `inProgress`, `succeeded`, `failed`, `unknownFutureValue`.|
|lastActionDateTime|DateTimeOffset||
|attemptsCount|Int32||
|targetResourceId|String||
|targetResourceLocation|String||
|error|[operationError](../resources/operationerror.md)||



## Response
If successful, this method returns a `201 Created` response code and a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsasyncoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/teams/{teamsId}/operations
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "operationType": "String",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:56:51.3643763+03:00",
  "attemptsCount": 13,
  "targetResourceId": "Target Resource Id value",
  "targetResourceLocation": "Target Resource Location value",
  "error": {
    "@odata.type": "microsoft.graph.operationError",
    "code": "Code value",
    "message": "Message value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 555

{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "id": "a94ec541-c541-a94e-41c5-4ea941c54ea9",
  "operationType": "String",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "status": "String",
  "lastActionDateTime": "2016-12-31T23:56:51.3643763+03:00",
  "attemptsCount": 13,
  "targetResourceId": "Target Resource Id value",
  "targetResourceLocation": "Target Resource Location value",
  "error": {
    "@odata.type": "microsoft.graph.operationError",
    "code": "Code value",
    "message": "Message value"
  }
}
```

