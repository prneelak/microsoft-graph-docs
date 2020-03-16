---
title: "deviceComplianceDeviceOverview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceDeviceOverview resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|
|[Update deviceComplianceDeviceOverview](../api/devicecompliancedeviceoverview-update.md)|[deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md)|Update the properties of a [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationVersion|Int32|Version of the policy for that overview|
|errorCount|Int32|Number of error devices|
|failedCount|Int32|Number of failed devices|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdateDateTime|DateTimeOffset|Last update time|
|notApplicableCount|Int32|Number of not applicable devices|
|pendingCount|Int32|Number of pending devices|
|successCount|Int32|Number of succeeded devices|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```

