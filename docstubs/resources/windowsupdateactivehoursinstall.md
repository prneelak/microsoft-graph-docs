---
title: "windowsUpdateActiveHoursInstall resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsUpdateActiveHoursInstall resource type


Namespace: microsoft.graph




Inherits from [windowsUpdateInstallScheduleType](../resources/windowsupdateinstallscheduletype.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeHoursEnd|TimeOfDay|Active Hours End|
|activeHoursStart|TimeOfDay|Active Hours Start|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```

