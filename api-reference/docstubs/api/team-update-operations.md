---
title: "Update operations"
description: "Update the properties of an operations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update operations

Namespace: microsoft.graph

Update the properties of an operations object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teams/{teamsId}/operations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.

The following table shows the properties that are required when you create the [teamsAsyncOperation](../resources/teamsasyncoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|operationType|teamsAsyncOperationType|**TODO: Add Description**. Possible values are: `invalid`, `cloneTeam`, `archiveTeam`, `unarchiveTeam`, `createTeam`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|status|teamsAsyncOperationStatus|**TODO: Add Description**. Possible values are: `invalid`, `notStarted`, `inProgress`, `succeeded`, `failed`, `unknownFutureValue`.|
|lastActionDateTime|DateTimeOffset|**TODO: Add Description**|
|attemptsCount|Int32|**TODO: Add Description**|
|targetResourceId|String|**TODO: Add Description**|
|targetResourceLocation|String|**TODO: Add Description**|
|error|[operationError](../resources/operationerror.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsAsyncOperation](../resources/teamsasyncoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_operations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/operations
Content-Type: application/json
Content-length: 337

{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "operationType": "String",
  "status": "String",
  "lastActionDateTime": "String (timestamp)",
  "attemptsCount": "Integer",
  "targetResourceId": "String",
  "targetResourceLocation": "String",
  "error": {
    "@odata.type": "microsoft.graph.operationError"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "id": "07aae04d-e04d-07aa-4de0-aa074de0aa07",
  "operationType": "String",
  "createdDateTime": "String (timestamp)",
  "status": "String",
  "lastActionDateTime": "String (timestamp)",
  "attemptsCount": "Integer",
  "targetResourceId": "String",
  "targetResourceLocation": "String",
  "error": {
    "@odata.type": "microsoft.graph.operationError"
  }
}
```

