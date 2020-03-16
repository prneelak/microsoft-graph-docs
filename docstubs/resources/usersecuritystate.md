---
title: "userSecurityState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userSecurityState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|aadUserId|String||
|accountName|String||
|domainName|String||
|emailRole|Enumeration|. Possible values are: `unknown`, `sender`, `recipient`, `unknownFutureValue`.|
|isVpn|Boolean||
|logonDateTime|DateTimeOffset||
|logonId|String||
|logonIp|String||
|logonLocation|String||
|logonType|Enumeration|. Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`, `unknownFutureValue`.|
|onPremisesSecurityIdentifier|String||
|riskScore|String||
|userAccountType|Enumeration|. Possible values are: `unknown`, `standard`, `power`, `administrator`, `unknownFutureValue`.|
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSecurityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSecurityState",
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "String",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "String",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "String",
  "userPrincipalName": "String"
}
```

