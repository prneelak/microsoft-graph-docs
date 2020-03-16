---
title: "deviceConfigurationState resource type"
description: "Device Configuration State for a given device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationState resource type


Namespace: microsoft.graph

Device Configuration State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationState](../api/deviceconfigurationstate-get.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Read properties and relationships of the [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|
|[Update deviceConfigurationState](../api/deviceconfigurationstate-update.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Update the properties of a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|
|[List deviceConfigurationStates](../api/manageddevice-list-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Get the deviceConfigurationStates from the deviceConfigurationStates navigation property.|
|[Add deviceConfigurationStates](../api/manageddevice-post-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Add deviceConfigurationStates by posting to the deviceConfigurationStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the policy for this policyBase|
|id|String| Inherited from [entity](../resources/entity.md)|
|platformType|Enumeration|Platform type that the policy applies to. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|settingCount|Int32|Count of how many setting a policy holds|
|settingStates|[deviceConfigurationSettingState](../resources/deviceconfigurationsettingstate.md) collection||
|state|Enumeration|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|version|Int32|The version of the policy|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```

