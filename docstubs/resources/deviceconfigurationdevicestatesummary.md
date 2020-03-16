---
title: "deviceConfigurationDeviceStateSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationDeviceStateSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationDeviceStateSummary](../api/deviceconfigurationdevicestatesummary-get.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)|Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.|
|[Update deviceConfigurationDeviceStateSummary](../api/deviceconfigurationdevicestatesummary-update.md)|[deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md)|Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/deviceconfigurationdevicestatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|Number of compliant devices|
|conflictDeviceCount|Int32|Number of conflict devices|
|errorDeviceCount|Int32|Number of error devices|
|id|String| Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|unknownDeviceCount|Int32|Number of unknown devices|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```

