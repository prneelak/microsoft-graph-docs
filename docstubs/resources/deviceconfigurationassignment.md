---
title: "deviceConfigurationAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationAssignment](../api/deviceconfigurationassignment-get.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Read properties and relationships of the [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|
|[Update deviceConfigurationAssignment](../api/deviceconfigurationassignment-update.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Update the properties of a [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|
|[List assignments](../api/deviceconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|source|Enumeration| Possible values are: `direct`, `policySets`.|
|sourceId|String||
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```

