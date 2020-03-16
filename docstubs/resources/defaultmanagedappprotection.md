---
title: "defaultManagedAppProtection resource type"
description: "Policy used to configure detailed management settings for a specified set of apps for all users not targeted by a TargetedManagedAppProtection Policy"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# defaultManagedAppProtection resource type


Namespace: microsoft.graph

Policy used to configure detailed management settings for a specified set of apps for all users not targeted by a TargetedManagedAppProtection Policy


Inherits from [managedAppProtection](../resources/managedappprotection.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get defaultManagedAppProtection](../api/defaultmanagedappprotection-get.md)|[defaultManagedAppProtection](../resources/defaultmanagedappprotection.md)|Read properties and relationships of the [defaultManagedAppProtection](../resources/defaultmanagedappprotection.md) object.|
|[Update defaultManagedAppProtection](../api/defaultmanagedappprotection-update.md)|[defaultManagedAppProtection](../resources/defaultmanagedappprotection.md)|Update the properties of a [defaultManagedAppProtection](../resources/defaultmanagedappprotection.md) object.|
|[targetApps](../api/defaultmanagedappprotection-targetapps.md)|None||
|[List apps](../api/defaultmanagedappprotection-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Add apps](../api/defaultmanagedappprotection-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Add apps by posting to the apps collection.|
|[Get managedAppPolicyDeploymentSummary](../api/managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedDataStorageLocations|Enumeration collection|Data storage locations where a user may store managed data. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedInboundDataTransferSources|Enumeration|Sources from which data is allowed to be transferred. Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|allowedOutboundClipboardSharingLevel|Enumeration|The level to which the clipboard may be shared between apps on the managed device. Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|allowedOutboundDataTransferDestinations|Enumeration|Destinations to which data is allowed to be transferred. Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|appDataEncryptionType|Enumeration|Type of encryption which should be used for data in a managed app. (iOS Only). Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|contactSyncBlocked|Boolean|Indicates whether contacts can be synced to the user's device. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|createdDateTime|DateTimeOffset|The date and time the policy was created. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/keyvaluepair.md) collection|A set of string key and string value pairs to be sent to the affected users, unalterned by this service|
|dataBackupBlocked|Boolean|Indicates whether the backup of a managed app's data is blocked. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|deployedAppCount|Int32|Count of apps to which the current policy is deployed.|
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|deviceComplianceRequired|Boolean|Indicates whether device compliance is required. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|When this setting is enabled, app level encryption is disabled if device level encryption is enabled. (Android only)|
|disableAppPinIfDevicePinIsSet|Boolean|Indicates whether use of the app pin is required if the device pin is set. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|encryptAppData|Boolean|Indicates whether managed-app data should be encrypted. (Android only)|
|faceIdBlocked|Boolean|Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True. (iOS Only)|
|fingerprintBlocked|Boolean|Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|managedBrowserToOpenLinksRequired|Boolean|Indicates whether internet links should be opened in the managed browser app. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|maximumPinRetries|Int32|Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumPinLength|Int32|Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredAppVersion|String|Versions less than the specified version will block the managed app from accessing company data. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredOsVersion|String|Versions less than the specified version will block the managed app from accessing company data. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredPatchVersion|String|Define the oldest required Android security patch level a user can have to gain secure access to the app. (Android only)|
|minimumRequiredSdkVersion|String|Versions less than the specified version will block the managed app from accessing company data. (iOS Only)|
|minimumWarningAppVersion|String|Versions less than the specified version will result in warning message on the managed app. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningOsVersion|String|Versions less than the specified version will result in warning message on the managed app from accessing company data. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningPatchVersion|String|Define the oldest recommended Android security patch level a user can have for secure access to the app. (Android only)|
|organizationalCredentialsRequired|Boolean|Indicates whether organizational credentials are required for app use. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodBeforePinReset|Duration|TimePeriod before the all-level pin must be reset if PinRequired is set to True. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeAccessCheck|Duration|The period after which access is checked when the device is not connected to the internet. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration|The period after which access is checked when the device is connected to the internet. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinCharacterSet|Enumeration|Character set which may be used for an app-level pin if PinRequired is set to True. Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `numeric`, `alphanumericAndSymbol`.|
|pinRequired|Boolean|Indicates whether an app-level pin is required. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|printBlocked|Boolean|Indicates whether printing is allowed from managed apps. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|saveAsBlocked|Boolean|Indicates whether users may use the "Save As" menu item to save a copy of protected files. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|screenCaptureBlocked|Boolean|Indicates whether screen capture is blocked. (Android only)|
|simplePinBlocked|Boolean|Indicates whether simplePin is blocked. Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|version|String|Version of the entity. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|apps|[managedMobileApp](../resources/managedmobileapp.md) collection|List of apps to which the policy is deployed.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md)|Navigation property to deployment summary of the configuration.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection",
  "baseType": "microsoft.graph.managedAppProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "appDataEncryptionType": "String",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "faceIdBlocked": true
}
```

