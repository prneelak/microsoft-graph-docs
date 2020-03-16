---
title: "mobileThreatDefenseConnector resource type"
description: "Entity which represents a connection to Mobile threat defense partner."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileThreatDefenseConnector resource type


Namespace: microsoft.graph

Entity which represents a connection to Mobile threat defense partner.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileThreatDefenseConnector](../api/mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Read properties and relationships of the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|
|[Update mobileThreatDefenseConnector](../api/mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Update the properties of a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidDeviceBlockedOnMissingPartnerData|Boolean|For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant|
|androidEnabled|Boolean|For Android, set whether data from the data sync partner should be used during compliance evaluations|
|id|String| Inherited from [entity](../resources/entity.md)|
|iosDeviceBlockedOnMissingPartnerData|Boolean|For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant|
|iosEnabled|Boolean|For IOS, get or set whether data from the data sync partner should be used during compliance evaluations|
|lastHeartbeatDateTime|DateTimeOffset|DateTime of last Heartbeat recieved from the Data Sync Partner|
|partnerState|Enumeration|Data Sync Partner state for this account. Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.|
|partnerUnresponsivenessThresholdInDays|Int32|Get or Set days the per tenant tolerance to unresponsiveness for this partner integration|
|partnerUnsupportedOsVersionBlocked|Boolean|Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024
}
```

