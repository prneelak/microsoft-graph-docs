---
title: "managedEBookAssignment resource type"
description: "Contains properties used to assign a eBook to a group."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedEBookAssignment resource type


Namespace: microsoft.graph

Contains properties used to assign a eBook to a group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBookAssignment](../api/managedebookassignment-get.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Read properties and relationships of the [managedEBookAssignment](../resources/managedebookassignment.md) object.|
|[Update managedEBookAssignment](../api/managedebookassignment-update.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Update the properties of a [managedEBookAssignment](../resources/managedebookassignment.md) object.|
|[List assignments](../api/managedebook-list-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md) collection|Get the managedEBookAssignments from the assignments navigation property.|
|[Add assignments](../api/managedebook-post-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installIntent|Enumeration|The install intent for eBook. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The assignment target for eBook.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```

