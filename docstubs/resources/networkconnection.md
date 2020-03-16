---
title: "networkConnection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# networkConnection resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationName|String||
|destinationAddress|String||
|destinationDomain|String||
|destinationPort|String||
|destinationUrl|String||
|direction|Enumeration|. Possible values are: `unknown`, `inbound`, `outbound`, `unknownFutureValue`.|
|domainRegisteredDateTime|DateTimeOffset||
|localDnsName|String||
|natDestinationAddress|String||
|natDestinationPort|String||
|natSourceAddress|String||
|natSourcePort|String||
|protocol|Enumeration|. Possible values are: `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`, `unknownFutureValue`, `unknown`.|
|riskScore|String||
|sourceAddress|String||
|sourcePort|String||
|status|Enumeration|. Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`, `unknownFutureValue`.|
|urlParameters|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.networkConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkConnection",
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "String",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "String",
  "urlParameters": "String"
}
```

