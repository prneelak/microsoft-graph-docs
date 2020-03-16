---
title: "deviceComplianceSettingState resource type"
description: "Device compliance setting State for a given device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceSettingState resource type


Namespace: microsoft.graph

Device compliance setting State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceSettingState](../api/devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Read properties and relationships of the [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|
|[Update deviceComplianceSettingState](../api/devicecompliancesettingstate-update.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Update the properties of a [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|
|[List deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-list-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection|Get the deviceComplianceSettingStates from the deviceComplianceSettingStates navigation property.|
|[Add deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-post-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Add deviceComplianceSettingStates by posting to the deviceComplianceSettingStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|deviceId|String|The Device Id that is being reported|
|deviceModel|String|The device model that is being reported|
|deviceName|String|The Device Name that is being reported|
|id|String| Inherited from [entity](../resources/entity.md)|
|setting|String|The setting class name and property name.|
|settingName|String|The Setting Name that is being reported|
|state|Enumeration|The compliance state of the setting. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userEmail|String|The User email address that is being reported|
|userId|String|The user Id that is being reported|
|userName|String|The User Name that is being reported|
|userPrincipalName|String|The User PrincipalName that is being reported|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```

