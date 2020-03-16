---
title: "iosVppAppAssignmentSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosVppAppAssignmentSettings resource type


Namespace: microsoft.graph




Inherits from [mobileAppAssignmentSettings](../resources/mobileappassignmentsettings.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|useDeviceLicensing|Boolean|Whether or not to use device licensing.|
|vpnConfigurationId|String|The VPN Configuration Id to apply for this app.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```

