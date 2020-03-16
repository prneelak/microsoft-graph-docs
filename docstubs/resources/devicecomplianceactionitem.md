---
title: "deviceComplianceActionItem resource type"
description: "Scheduled Action Configuration"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceActionItem resource type


Namespace: microsoft.graph

Scheduled Action Configuration


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceActionItem](../api/devicecomplianceactionitem-get.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Read properties and relationships of the [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) object.|
|[Update deviceComplianceActionItem](../api/devicecomplianceactionitem-update.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Update the properties of a [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) object.|
|[List scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-list-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) collection|Get the deviceComplianceActionItems from the scheduledActionConfigurations navigation property.|
|[Add scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-post-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Add scheduledActionConfigurations by posting to the scheduledActionConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionType|Enumeration|What action to take. Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.|
|gracePeriodHours|Int32|Number of hours to wait till the action will be enforced. Valid values 0 to 8760|
|id|String| Inherited from [entity](../resources/entity.md)|
|notificationMessageCCList|String collection|A list of group IDs to speicify who to CC this notification message to.|
|notificationTemplateId|String|What notification Message template to use|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```

