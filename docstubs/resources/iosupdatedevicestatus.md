---
title: "iosUpdateDeviceStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosUpdateDeviceStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get iosUpdateDeviceStatus](../api/iosupdatedevicestatus-get.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md)|Read properties and relationships of the [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object.|
|[Update iosUpdateDeviceStatus](../api/iosupdatedevicestatus-update.md)|[iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md)|Update the properties of a [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|deviceDisplayName|String|Device name of the DevicePolicyStatus.|
|deviceId|String|The device id that is being reported.|
|deviceModel|String|The device model that is being reported|
|id|String| Inherited from [entity](../resources/entity.md)|
|installStatus|Enumeration|The installation status of the policy report. Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|osVersion|String|The device version that is being reported.|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userId|String|The User id that is being reported.|
|userName|String|The User Name that is being reported|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "String (identifier)",
  "installStatus": "String",
  "osVersion": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```

