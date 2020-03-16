---
title: "windowsInformationProtectionNetworkLearningSummary resource type"
description: "Windows Information Protection Network learning Summary entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionNetworkLearningSummary resource type


Namespace: microsoft.graph

Windows Information Protection Network learning Summary entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionNetworkLearningSummary](../api/windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.|
|[Update windowsInformationProtectionNetworkLearningSummary](../api/windowsinformationprotectionnetworklearningsummary-update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md)|Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/windowsinformationprotectionnetworklearningsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int32|Device Count|
|id|String| Inherited from [entity](../resources/entity.md)|
|url|String|Website url|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```

