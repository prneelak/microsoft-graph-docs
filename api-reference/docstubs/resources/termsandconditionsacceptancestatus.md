---
title: "termsAndConditionsAcceptanceStatus resource type"
description: "A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user. Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# termsAndConditionsAcceptanceStatus resource type


Namespace: microsoft.graph

A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user. Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditionsAcceptanceStatus](../api/termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Read properties and relationships of a [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.|
|[Update termsAndConditionsAcceptanceStatus](../api/termsandconditionsacceptancestatus-update.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) object.|
|[List termsAndConditions](../api/termsandconditionsacceptancestatus-list-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get the termsAndConditions from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/termsandconditionsacceptancestatus-post-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|
|[Remove termsAndConditions](../api/termsandconditionsacceptancestatus-delete-termsandconditions.md)|None|Remove a termsAndConditions object.|
|[List acceptanceStatuses](../api/termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatus from the acceptanceStatuses navigation property.|
|[Create acceptanceStatuses](../api/termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Create a new acceptanceStatuses object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptedDateTime|DateTimeOffset|DateTime when the terms were last accepted by the user.|
|acceptedVersion|Int32|Most recent version number of the T&C accepted by the user.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userDisplayName|String|Display name of the user whose acceptance the entity represents.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md)|Navigation link to the terms and conditions that are assigned.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```

