---
title: "deviceManagementTroubleshootingEvent resource type"
description: "Event representing an general failure."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementTroubleshootingEvent resource type


Namespace: microsoft.graph

Event representing an general failure.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementTroubleshootingEvent](../api/devicemanagementtroubleshootingevent-get.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.|
|[Update deviceManagementTroubleshootingEvent](../api/devicemanagementtroubleshootingevent-update.md)|[deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|Update the properties of a [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|correlationId|String|Id used for tracing the failure in the service.|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String"
}
```

