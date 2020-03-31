---
title: "Delete governanceRoleDefinition"
description: "Deletes a governanceRoleDefinition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete governanceRoleDefinition

Namespace: microsoft.graph

Deletes a [governanceRoleDefinition](../resources/governanceroledefinition.md).

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
DELETE /governanceRoleDefinitions/{governanceRoleDefinitionsId}
DELETE /governanceRoleSettings/{governanceRoleSettingsId}/roleDefinition
DELETE /governanceRoleAssignments/{governanceRoleAssignmentsId}/roleDefinition
DELETE /privilegedAccess/{privilegedAccessId}/roleDefinitions/{governanceRoleDefinitionId}
DELETE /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/roleDefinition
DELETE /governanceResources/{governanceResourcesId}/roleDefinitions/{governanceRoleDefinitionId}
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}/roleDefinition
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/roleSetting/roleDefinition
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/roleDefinition
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_governanceroledefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/governanceRoleDefinitions/{governanceRoleDefinitionsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

