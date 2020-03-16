---
title: "remoteAssistancePartner resource type"
description: "remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# remoteAssistancePartner resource type


Namespace: microsoft.graph

remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get remoteAssistancePartner](../api/remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Read properties and relationships of the [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.|
|[Update remoteAssistancePartner](../api/remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/remoteassistancepartner.md)|Update the properties of a [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.|
|[beginOnboarding](../api/remoteassistancepartner-beginonboarding.md)|None||
|[disconnect](../api/remoteassistancepartner-disconnect.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Display name of the partner.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastConnectionDateTime|DateTimeOffset|Timestamp of the last request sent to Intune by the TEM partner.|
|onboardingStatus|Enumeration|TBD. Possible values are: `notOnboarded`, `onboarding`, `onboarded`.|
|onboardingUrl|String|URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```

