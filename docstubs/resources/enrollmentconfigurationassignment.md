---
title: "enrollmentConfigurationAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# enrollmentConfigurationAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-get.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[Update enrollmentConfigurationAssignment](../api/enrollmentconfigurationassignment-update.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Update the properties of a [enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) object.|
|[List assignments](../api/deviceenrollmentconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceenrollmentconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

