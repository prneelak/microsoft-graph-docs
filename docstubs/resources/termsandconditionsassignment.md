---
title: "termsAndConditionsAssignment resource type"
description: "A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# termsAndConditionsAssignment resource type


Namespace: microsoft.graph

A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditionsAssignment](../api/termsandconditionsassignment-get.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Read properties and relationships of the [termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) object.|
|[Update termsAndConditionsAssignment](../api/termsandconditionsassignment-update.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Update the properties of a [termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) object.|
|[List assignments](../api/termsandconditions-list-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|Get the termsAndConditionsAssignments from the assignments navigation property.|
|[Add assignments](../api/termsandconditions-post-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|Assignment target that the T&C policy is assigned to.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

