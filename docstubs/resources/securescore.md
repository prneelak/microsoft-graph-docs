---
title: "secureScore resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# secureScore resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get secureScore](../api/securescore-get.md)|[secureScore](../resources/securescore.md)|Read properties and relationships of the [secureScore](../resources/securescore.md) object.|
|[Update secureScore](../api/securescore-update.md)|[secureScore](../resources/securescore.md)|Update the properties of a [secureScore](../resources/securescore.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeUserCount|Int32||
|averageComparativeScores|[averageComparativeScore](../resources/averagecomparativescore.md) collection||
|azureTenantId|String||
|controlScores|[controlScore](../resources/controlscore.md) collection||
|createdDateTime|DateTimeOffset||
|currentScore|Double||
|enabledServices|String collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|licensedUserCount|Int32||
|maxScore|Double||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.secureScore",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.secureScore",
  "id": "String (identifier)",
  "activeUserCount": 1024,
  "averageComparativeScores": [
    {
      "@odata.type": "microsoft.graph.averageComparativeScore"
    }
  ],
  "azureTenantId": "String",
  "controlScores": [
    {
      "@odata.type": "microsoft.graph.controlScore"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "currentScore": "Double",
  "enabledServices": [
    "String"
  ],
  "licensedUserCount": 1024,
  "maxScore": "Double",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

