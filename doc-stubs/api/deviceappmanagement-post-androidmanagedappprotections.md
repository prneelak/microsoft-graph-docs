---
title: "Create androidManagedAppProtections"
description: "Create a new androidManagedAppProtections object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create androidManagedAppProtections

Namespace: microsoft.graph

Create a new androidManagedAppProtections object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/androidManagedAppProtections
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object.

The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/androidmanagedappprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|description|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|roleScopeTagIds|String collection|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|version|String|**TODO: Add Description** Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedInboundDataTransferSources|managedAppDataTransferLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|managedAppDataTransferLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|managedAppClipboardSharingLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|deviceComplianceRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|saveAsBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinRequired|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|maximumPinRetries|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|simplePinBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumPinLength|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|pinCharacterSet|managedAppPinCharacterSet|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedDataStorageLocations|managedAppDataStorageLocation collection|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.|
|contactSyncBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|printBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|fingerprintBlocked|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredOsVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningOsVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumRequiredAppVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWarningAppVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeOsVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|minimumWipeAppVersion|String|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|appActionIfDeviceComplianceRequired|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|appActionIfMaximumPinRetriesExceeded|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedOutboundClipboardSharingExceptionLength|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|notificationRestriction|managedAppNotificationRestriction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `allow`, `blockOrganizationalData`, `block`.|
|previousPinBlockCount|Int32|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|managedBrowser|managedBrowserType|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `microsoftEdge`.|
|maximumAllowedDeviceThreatLevel|managedAppDeviceThreatLevel|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `notConfigured`, `secured`, `low`, `medium`, `high`.|
|mobileThreatDefenseRemediationAction|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|blockDataIngestionIntoOrganizationDocuments|Boolean|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md)|
|allowedDataIngestionLocations|managedAppDataIngestionLocation collection|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `oneDriveForBusiness`, `sharePoint`, `camera`.|
|appActionIfUnableToAuthenticateUser|managedAppRemediationAction|**TODO: Add Description** Inherited from [managedAppProtection](../resources/managedappprotection.md). Possible values are: `block`, `wipe`, `warn`.|
|isAssigned|Boolean|**TODO: Add Description** Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md)|
|targetedAppManagementLevels|appManagementLevel|**TODO: Add Description** Inherited from [targetedManagedAppProtection](../resources/targetedmanagedappprotection.md). Possible values are: `unspecified`, `unmanaged`, `mdm`, `androidEnterprise`.|
|screenCaptureBlocked|Boolean|**TODO: Add Description**|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|**TODO: Add Description**|
|encryptAppData|Boolean|**TODO: Add Description**|
|deployedAppCount|Int32|**TODO: Add Description**|
|minimumRequiredPatchVersion|String|**TODO: Add Description**|
|minimumWarningPatchVersion|String|**TODO: Add Description**|
|exemptedAppPackages|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|minimumWipePatchVersion|String|**TODO: Add Description**|
|allowedAndroidDeviceManufacturers|String|**TODO: Add Description**|
|appActionIfAndroidDeviceManufacturerNotAllowed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetDeviceAttestationType|androidManagedAppSafetyNetDeviceAttestationType|**TODO: Add Description**. Possible values are: `none`, `basicIntegrity`, `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|androidManagedAppSafetyNetAppsVerificationType|**TODO: Add Description**. Possible values are: `none`, `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|
|customBrowserPackageId|String|**TODO: Add Description**|
|customBrowserDisplayName|String|**TODO: Add Description**|
|minimumRequiredCompanyPortalVersion|String|**TODO: Add Description**|
|minimumWarningCompanyPortalVersion|String|**TODO: Add Description**|
|minimumWipeCompanyPortalVersion|String|**TODO: Add Description**|
|keyboardsRestricted|Boolean|**TODO: Add Description**|
|approvedKeyboards|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|allowedAndroidDeviceModels|String collection|**TODO: Add Description**|
|appActionIfAndroidDeviceModelNotAllowed|managedAppRemediationAction|**TODO: Add Description**. Possible values are: `block`, `wipe`, `warn`.|



## Response

If successful, this method returns a `201 Created` response code and an [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_androidmanagedappprotection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
Content-Type: application/json
Content-length: 3325

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": "Boolean",
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": "Boolean",
  "deviceComplianceRequired": "Boolean",
  "managedBrowserToOpenLinksRequired": "Boolean",
  "saveAsBlocked": "Boolean",
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": "Boolean",
  "maximumPinRetries": "Integer",
  "simplePinBlocked": "Boolean",
  "minimumPinLength": "Integer",
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": "Boolean",
  "printBlocked": "Boolean",
  "fingerprintBlocked": "Boolean",
  "disableAppPinIfDevicePinIsSet": "Boolean",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": "Integer",
  "notificationRestriction": "String",
  "previousPinBlockCount": "Integer",
  "managedBrowser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "blockDataIngestionIntoOrganizationDocuments": "Boolean",
  "allowedDataIngestionLocations": [
    "String"
  ],
  "appActionIfUnableToAuthenticateUser": "String",
  "isAssigned": "Boolean",
  "targetedAppManagementLevels": "String",
  "screenCaptureBlocked": "Boolean",
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": "Boolean",
  "encryptAppData": "Boolean",
  "deployedAppCount": "Integer",
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "minimumWipePatchVersion": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String",
  "keyboardsRestricted": "Boolean",
  "approvedKeyboards": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "allowedAndroidDeviceModels": [
    "String"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidmanagedappprotection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "id": "871f8125-8125-871f-2581-1f8725811f87",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": "Boolean",
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": "Boolean",
  "deviceComplianceRequired": "Boolean",
  "managedBrowserToOpenLinksRequired": "Boolean",
  "saveAsBlocked": "Boolean",
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": "Boolean",
  "maximumPinRetries": "Integer",
  "simplePinBlocked": "Boolean",
  "minimumPinLength": "Integer",
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": "Boolean",
  "printBlocked": "Boolean",
  "fingerprintBlocked": "Boolean",
  "disableAppPinIfDevicePinIsSet": "Boolean",
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": "Integer",
  "notificationRestriction": "String",
  "previousPinBlockCount": "Integer",
  "managedBrowser": "String",
  "maximumAllowedDeviceThreatLevel": "String",
  "mobileThreatDefenseRemediationAction": "String",
  "blockDataIngestionIntoOrganizationDocuments": "Boolean",
  "allowedDataIngestionLocations": [
    "String"
  ],
  "appActionIfUnableToAuthenticateUser": "String",
  "isAssigned": "Boolean",
  "targetedAppManagementLevels": "String",
  "screenCaptureBlocked": "Boolean",
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": "Boolean",
  "encryptAppData": "Boolean",
  "deployedAppCount": "Integer",
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "minimumWipePatchVersion": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
  "customBrowserPackageId": "String",
  "customBrowserDisplayName": "String",
  "minimumRequiredCompanyPortalVersion": "String",
  "minimumWarningCompanyPortalVersion": "String",
  "minimumWipeCompanyPortalVersion": "String",
  "keyboardsRestricted": "Boolean",
  "approvedKeyboards": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "allowedAndroidDeviceModels": [
    "String"
  ],
  "appActionIfAndroidDeviceModelNotAllowed": "String"
}
```

