---
title: "Add roleAssignments"
description: "Add roleAssignments by posting to the roleAssignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add roleAssignments

Namespace: microsoft.graph

Add roleAssignments by posting to the roleAssignments collection.

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
POST /deviceManagement/roleAssignments/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object.

The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The display or friendly name of the role Assignment. Inherited from [roleAssignment](../resources/roleassignment.md)|
|description|String|Description of the Role Assignment. Inherited from [roleAssignment](../resources/roleassignment.md)|
|resourceScopes|String collection|List of ids of role scope member security groups.  These are IDs from Azure Active Directory. Inherited from [roleAssignment](../resources/roleassignment.md)|
|members|String collection|The list of ids of role member security groups. These are IDs from Azure Active Directory.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceandappmanagementroleassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceandappmanagementroleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "0ace3023-3023-0ace-2330-ce0a2330ce0a",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

