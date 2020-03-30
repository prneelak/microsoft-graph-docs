---
title: "Update privilegedRole"
description: "Update the properties of a privilegedRole object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedRole

Namespace: microsoft.graph

Update the properties of a [privilegedRole](../resources/privilegedrole.md) object.

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
PATCH /privilegedRoles/{privilegedRolesId}
PATCH /privilegedApproval/{privilegedApprovalId}/roleInfo
PATCH /privilegedApproval/{privilegedApprovalId}/request/roleInfo
PATCH /privilegedRoleAssignments/{privilegedRoleAssignmentsId}/roleInfo
PATCH /privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}/roleInfo
PATCH /privilegedRoles/{privilegedRolesId}/assignments/{privilegedRoleAssignmentId}/roleInfo
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedRole](../resources/privilegedrole.md) object.

The following table shows the properties that are required when you create the [privilegedRole](../resources/privilegedrole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedRole](../resources/privilegedrole.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedrole"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}
Content-type: application/json
Content-length: 81

{
  "@odata.type": "#microsoft.graph.privilegedRole",
  "name": "Name value"
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
Content-Length: 130

{
  "@odata.type": "#microsoft.graph.privilegedRole",
  "id": "a4ad95a0-95a0-a4ad-a095-ada4a095ada4",
  "name": "Name value"
}
```

