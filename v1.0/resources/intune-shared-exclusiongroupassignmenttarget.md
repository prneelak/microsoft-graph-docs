---
title: "exclusionGroupAssignmentTarget resource type"
description: "Represents a group that should be excluded from an assignment."
author: "davidmu1"
localization_priority: Normal
ms.prod: "Intune"
doc_type: resourcePageType
---

# exclusionGroupAssignmentTarget resource type

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Represents a group that should be excluded from an assignment.


Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|groupId|String|The group Id that is the target of the assignment. Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```




