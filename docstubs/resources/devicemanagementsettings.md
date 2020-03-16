---
title: "deviceManagementSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|The number of days a device is allowed to go without checking in to remain compliant. Valid values 0 to 120|
|isScheduledActionEnabled|Boolean|Is feature enabled or not for scheduled action for rule.|
|secureByDefault|Boolean|Device should be noncompliant when there is no compliance policy targeted when this is true|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```

