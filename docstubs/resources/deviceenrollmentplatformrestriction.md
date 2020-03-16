---
title: "deviceEnrollmentPlatformRestriction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceEnrollmentPlatformRestriction resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|osMaximumVersion|String|Max OS version supported|
|osMinimumVersion|String|Min OS version supported|
|personalDeviceEnrollmentBlocked|Boolean|Block personally owned devices from enrolling|
|platformBlocked|Boolean|Block the platform from enrolling|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```

