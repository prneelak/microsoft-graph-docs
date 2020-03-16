---
title: "roleDefinition resource type"
description: "The Role Definition resource. The role definition is the foundation of role based access in Intune. The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource. There are two types of roles, built-in and custom. Built-in roles cannot be modified. Both built-in roles and custom roles must have assignments to be enforced. Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleDefinition resource type


Namespace: microsoft.graph

The Role Definition resource. The role definition is the foundation of role based access in Intune. The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource. There are two types of roles, built-in and custom. Built-in roles cannot be modified. Both built-in roles and custom roles must have assignments to be enforced. Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleDefinition](../api/roledefinition-get.md)|[roleDefinition](../resources/roledefinition.md)|Read properties and relationships of the [roleDefinition](../resources/roledefinition.md) object.|
|[Update roleDefinition](../api/roledefinition-update.md)|[roleDefinition](../resources/roledefinition.md)|Update the properties of a [roleDefinition](../resources/roledefinition.md) object.|
|[List roleAssignments](../api/roledefinition-list-roleassignments.md)|[roleAssignment](../resources/roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/roledefinition-post-roleassignments.md)|[roleAssignment](../resources/roleassignment.md)|Add roleAssignments by posting to the roleAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description of the Role definition.|
|displayName|String|Display Name of the Role definition.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|Type of Role. Set to True if it is built-in, or set to False if it is a custom role definition.|
|rolePermissions|[rolePermission](../resources/rolepermission.md) collection|List of Role Permissions this role is allowed to perform. These must match the actionName that is defined as part of the rolePermission.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/roleassignment.md) collection|List of Role assignments for this role definition.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "isBuiltIn": true
}
```

