---
title: "Create operations"
description: "Create a new operations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create operations

Namespace: microsoft.graph

Create a new operations object.

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
POST /users/{usersId}/onenote/operations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onenoteOperation](../resources/onenoteoperation.md) object.

The following table shows the properties that are required when you create the [onenoteOperation](../resources/onenoteoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|operationStatus|**TODO: Add Description** Inherited from [operation](../resources/operation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [operation](../resources/operation.md)|
|lastActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [operation](../resources/operation.md)|
|resourceLocation|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|error|[onenoteOperationError](../resources/onenoteoperationerror.md)|**TODO: Add Description**|
|percentComplete|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [onenoteOperation](../resources/onenoteoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_onenoteoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/onenote/operations
Content-Type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "status": "String",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "resourceId": "String",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError"
  },
  "percentComplete": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "id": "965e5049-5049-965e-4950-5e9649505e96",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "resourceId": "String",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError"
  },
  "percentComplete": "String"
}
```

