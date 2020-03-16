---
title: "targetedManagedAppPolicyAssignment resource type"
description: "The type for deployment of groups or apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# targetedManagedAppPolicyAssignment resource type


Namespace: microsoft.graph

The type for deployment of groups or apps.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get targetedManagedAppPolicyAssignment](../api/targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|
|[Update targetedManagedAppPolicyAssignment](../api/targetedmanagedapppolicyassignment-update.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Update the properties of a [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|
|[List assignments](../api/androidmanagedappprotection-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Add assignments](../api/androidmanagedappprotection-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|Identifier for deployment of a group or app|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

