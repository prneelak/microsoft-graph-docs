---
title: "iosNotificationSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosNotificationSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|alertType|Enumeration|Indicates the type of alert for notifications for this app. Possible values are: `deviceDefault`, `banner`, `modal`, `none`.|
|appName|String|Application name to be associated with the bundleID.|
|badgesEnabled|Boolean|Indicates whether badges are allowed for this app.|
|bundleID|String|Bundle id of app to which to apply these notification settings.|
|enabled|Boolean|Indicates whether notifications are allowed for this app.|
|publisher|String|Publisher to be associated with the bundleID.|
|showInNotificationCenter|Boolean|Indicates whether notifications can be shown in notification center.|
|showOnLockScreen|Boolean|Indicates whether notifications can be shown on the lock screen.|
|soundsEnabled|Boolean|Indicates whether sounds are allowed for this app.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```

