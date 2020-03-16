---
title: "deviceOperatingSystemSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceOperatingSystemSummary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidCount|Int32|Number of android device count.|
|iosCount|Int32|Number of iOS device count.|
|macOSCount|Int32|Number of Mac OS X device count.|
|unknownCount|Int32|Number of unknown device count.|
|windowsCount|Int32|Number of Windows device count.|
|windowsMobileCount|Int32|Number of Windows mobile device count.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```

