---
title: "termsAndConditions resource type"
description: "A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy. T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance. They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# termsAndConditions resource type


Namespace: microsoft.graph

A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy. T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance. They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditions](../api/termsandconditions-get.md)|[termsAndConditions](../resources/termsandconditions.md)|Read properties and relationships of the [termsAndConditions](../resources/termsandconditions.md) object.|
|[Update termsAndConditions](../api/termsandconditions-update.md)|[termsAndConditions](../resources/termsandconditions.md)|Update the properties of a [termsAndConditions](../resources/termsandconditions.md) object.|
|[List assignments](../api/termsandconditions-list-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|Get the termsAndConditionsAssignments from the assignments navigation property.|
|[Add assignments](../api/termsandconditions-post-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Add assignments by posting to the assignments collection.|
|[List acceptanceStatuses](../api/termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatuses from the acceptanceStatuses navigation property.|
|[Add acceptanceStatuses](../api/termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Add acceptanceStatuses by posting to the acceptanceStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptanceStatement|String|Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy. This is shown to the user on prompts to accept the T&C policy.|
|bodyText|String|Administrator-supplied body text of the terms and conditions, typically the terms themselves. This is shown to the user on prompts to accept the T&C policy.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Administrator-supplied description of the T&C policy.|
|displayName|String|Administrator-supplied name for the T&C policy. |
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|title|String|Administrator-supplied title of the terms and conditions. This is shown to the user on prompts to accept the T&C policy.|
|version|Int32|Integer indicating the current version of the terms. Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|The list of acceptance statuses for this T&C policy.|
|assignments|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|The list of assignments for this T&C policy.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```

