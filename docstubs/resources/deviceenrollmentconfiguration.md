---
title: "deviceEnrollmentConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceEnrollmentConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceEnrollmentConfiguration](../api/deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object.|
|[setPriority](../api/deviceenrollmentconfiguration-setpriority.md)|None||
|[assign](../api/deviceenrollmentconfiguration-assign.md)|None||
|[List assignments](../api/deviceenrollmentconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceenrollmentconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|priority|Int32||
|version|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|The list of group assignments for the device configuration profile.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```

