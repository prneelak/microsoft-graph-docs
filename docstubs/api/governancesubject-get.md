---
title: "Get governanceSubject"
description: "Read properties and relationships of the governanceSubject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get governanceSubject

Namespace: microsoft.graph

Read properties and relationships of the [governanceSubject](../resources/governancesubject.md) object.

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
GET /governanceSubjects/{governanceSubjectsId}
GET /governanceRoleAssignments/{governanceRoleAssignmentsId}/subject
GET /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/subject
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}/subject
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/subject
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
If successful, this method returns a `200 OK` response code and [governanceSubject](../resources/governancesubject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_governancesubject"
}
-->
``` http
GET https://graph.microsoft.com/beta/governanceSubjects/{governanceSubjectsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceSubject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": {
    "@odata.type": "#microsoft.graph.governanceSubject",
    "id": "cfab5d64-5d64-cfab-645d-abcf645dabcf",
    "type": "Type value",
    "displayName": "Display Name value",
    "principalName": "Principal Name value",
    "email": "Email value"
  }
}
```

