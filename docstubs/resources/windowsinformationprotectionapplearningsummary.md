---
title: "windowsInformationProtectionAppLearningSummary resource type"
description: "Windows Information Protection AppLearning Summary entity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionAppLearningSummary resource type


Namespace: microsoft.graph

Windows Information Protection AppLearning Summary entity.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionAppLearningSummary](../api/windowsinformationprotectionapplearningsummary-get.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Read properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.|
|[Update windowsInformationProtectionAppLearningSummary](../api/windowsinformationprotectionapplearningsummary-update.md)|[windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md)|Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationName|String|Application Name|
|applicationType|Enumeration|Application Type. Possible values are: `universal`, `desktop`.|
|deviceCount|Int32|Device Count|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```

