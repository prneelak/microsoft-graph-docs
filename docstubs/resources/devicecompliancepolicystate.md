---
title: "deviceCompliancePolicyState resource type"
description: "Device Compliance Policy State for a given device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceCompliancePolicyState resource type


Namespace: microsoft.graph

Device Compliance Policy State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicyState](../api/devicecompliancepolicystate-get.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Read properties and relationships of the [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.|
|[Update deviceCompliancePolicyState](../api/devicecompliancepolicystate-update.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Update the properties of a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.|
|[List deviceCompliancePolicyStates](../api/manageddevice-list-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.|
|[Add deviceCompliancePolicyStates](../api/manageddevice-post-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Add deviceCompliancePolicyStates by posting to the deviceCompliancePolicyStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the policy for this policyBase|
|id|String| Inherited from [entity](../resources/entity.md)|
|platformType|Enumeration|Platform type that the policy applies to. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|settingCount|Int32|Count of how many setting a policy holds|
|settingStates|[deviceCompliancePolicySettingState](../resources/devicecompliancepolicysettingstate.md) collection||
|state|Enumeration|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|version|Int32|The version of the policy|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```

