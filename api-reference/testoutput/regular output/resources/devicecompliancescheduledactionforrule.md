---
title: "deviceComplianceScheduledActionForRule resource type"
description: "Scheduled Action for Rule"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceScheduledActionForRule resource type


Namespace: microsoft.graph

Scheduled Action for Rule


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceComplianceScheduledActionForRules](../api/devicecompliancescheduledactionforrule-list.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) collection|List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) objects.|
|[Get deviceComplianceScheduledActionForRule](../api/devicecompliancescheduledactionforrule-get.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.|
|[Create deviceComplianceScheduledActionForRule](../api/devicecompliancescheduledactionforrule-create.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Create a new [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.|
|[Delete deviceComplianceScheduledActionForRule](../api/devicecompliancescheduledactionforrule-delete.md)|None|Deletes a [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md).|
|[Update deviceComplianceScheduledActionForRule](../api/devicecompliancescheduledactionforrule-update.md)|[deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md)|Update the properties of a [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.|
|[List scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-list-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) collection|Get the deviceComplianceActionItems from the scheduledActionConfigurations navigation property.|
|[Add scheduledActionConfigurations](../api/devicecompliancescheduledactionforrule-post-scheduledactionconfigurations.md)|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md)|Add scheduledActionConfigurations by posting to the scheduledActionConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|ruleName|String|Name of the rule which this scheduled action applies to.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|scheduledActionConfigurations|[deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) collection|The list of scheduled action configurations for this compliance policy.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```

