---
title: "deviceCompliancePolicySettingStateSummary resource type"
description: "Device Compilance Policy Setting State summary across the account."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceCompliancePolicySettingStateSummary resource type


Namespace: microsoft.graph

Device Compilance Policy Setting State summary across the account.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicySettingStateSummary](../api/devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.|
|[Update deviceCompliancePolicySettingStateSummary](../api/devicecompliancepolicysettingstatesummary-update.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.|
|[List deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-list-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection|Get the deviceComplianceSettingStates from the deviceComplianceSettingStates navigation property.|
|[Add deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-post-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Add deviceComplianceSettingStates by posting to the deviceComplianceSettingStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|Number of compliant devices|
|conflictDeviceCount|Int32|Number of conflict devices|
|errorDeviceCount|Int32|Number of error devices|
|id|String| Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|platformType|Enumeration|Setting platform. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|remediatedDeviceCount|Int32|Number of remediated devices|
|setting|String|The setting class name and property name.|
|settingName|String|Name of the setting.|
|unknownDeviceCount|Int32|Number of unknown devices|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceComplianceSettingStates|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```

