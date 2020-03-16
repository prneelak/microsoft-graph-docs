---
title: "deviceExchangeAccessStateSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceExchangeAccessStateSummary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedDeviceCount|Int32|Total count of devices with Exchange Access State: Allowed.|
|blockedDeviceCount|Int32|Total count of devices with Exchange Access State: Blocked.|
|quarantinedDeviceCount|Int32|Total count of devices with Exchange Access State: Quarantined.|
|unavailableDeviceCount|Int32|Total count of devices for which no Exchange Access State could be found.|
|unknownDeviceCount|Int32|Total count of devices with Exchange Access State: Unknown.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```

