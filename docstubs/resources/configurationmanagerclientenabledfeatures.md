---
title: "configurationManagerClientEnabledFeatures resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# configurationManagerClientEnabledFeatures resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliancePolicy|Boolean|Whether compliance policy is managed by Intune|
|deviceConfiguration|Boolean|Whether device configuration is managed by Intune|
|inventory|Boolean|Whether inventory is managed by Intune|
|modernApps|Boolean|Whether modern application is managed by Intune|
|resourceAccess|Boolean|Whether resource access is managed by Intune|
|windowsUpdateForBusiness|Boolean|Whether Windows Update for Business is managed by Intune|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```

