---
title: "secureScoreControlProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# secureScoreControlProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get secureScoreControlProfile](../api/securescorecontrolprofile-get.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Read properties and relationships of the [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.|
|[Update secureScoreControlProfile](../api/securescorecontrolprofile-update.md)|[secureScoreControlProfile](../resources/securescorecontrolprofile.md)|Update the properties of a [secureScoreControlProfile](../resources/securescorecontrolprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionType|String||
|actionUrl|String||
|azureTenantId|String||
|complianceInformation|[complianceInformation](../resources/complianceinformation.md) collection||
|controlCategory|String||
|controlStateUpdates|[secureScoreControlStateUpdate](../resources/securescorecontrolstateupdate.md) collection||
|deprecated|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|implementationCost|String||
|lastModifiedDateTime|DateTimeOffset||
|maxScore|Double||
|rank|Int32||
|remediation|String||
|remediationImpact|String||
|service|String||
|threats|String collection||
|tier|String||
|title|String||
|userImpact|String||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.secureScoreControlProfile",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.secureScoreControlProfile",
  "id": "String (identifier)",
  "actionType": "String",
  "actionUrl": "String",
  "azureTenantId": "String",
  "complianceInformation": [
    {
      "@odata.type": "microsoft.graph.complianceInformation"
    }
  ],
  "controlCategory": "String",
  "controlStateUpdates": [
    {
      "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
    }
  ],
  "deprecated": true,
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": 1024,
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": [
    "String"
  ],
  "tier": "String",
  "title": "String",
  "userImpact": "String",
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```

