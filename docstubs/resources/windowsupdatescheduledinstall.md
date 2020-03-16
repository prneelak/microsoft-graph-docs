---
title: "windowsUpdateScheduledInstall resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsUpdateScheduledInstall resource type


Namespace: microsoft.graph




Inherits from [windowsUpdateInstallScheduleType](../resources/windowsupdateinstallscheduletype.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|scheduledInstallDay|Enumeration|Scheduled Install Day in week. Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|scheduledInstallTime|TimeOfDay|Scheduled Install Time during day|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```

