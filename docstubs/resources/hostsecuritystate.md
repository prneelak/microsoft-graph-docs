---
title: "hostSecurityState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# hostSecurityState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|fqdn|String||
|isAzureAdJoined|Boolean||
|isAzureAdRegistered|Boolean||
|isHybridAzureDomainJoined|Boolean||
|netBiosName|String||
|os|String||
|privateIpAddress|String||
|publicIpAddress|String||
|riskScore|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hostSecurityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hostSecurityState",
  "fqdn": "String",
  "isAzureAdJoined": true,
  "isAzureAdRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}
```

