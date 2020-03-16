---
title: "managedDevice resource type"
description: "Devices that are managed or pre-enrolled through Intune"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDevice resource type


Namespace: microsoft.graph

Devices that are managed or pre-enrolled through Intune


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read properties and relationships of the [managedDevice](../resources/manageddevice.md) object.|
|[Update managedDevice](../api/manageddevice-update.md)|[managedDevice](../resources/manageddevice.md)|Update the properties of a [managedDevice](../resources/manageddevice.md) object.|
|[retire](../api/manageddevice-retire.md)|None||
|[wipe](../api/manageddevice-wipe.md)|None||
|[resetPasscode](../api/manageddevice-resetpasscode.md)|None||
|[remoteLock](../api/manageddevice-remotelock.md)|None||
|[requestRemoteAssistance](../api/manageddevice-requestremoteassistance.md)|None||
|[disableLostMode](../api/manageddevice-disablelostmode.md)|None||
|[locateDevice](../api/manageddevice-locatedevice.md)|None||
|[bypassActivationLock](../api/manageddevice-bypassactivationlock.md)|None||
|[rebootNow](../api/manageddevice-rebootnow.md)|None||
|[shutDown](../api/manageddevice-shutdown.md)|None||
|[recoverPasscode](../api/manageddevice-recoverpasscode.md)|None||
|[cleanWindowsDevice](../api/manageddevice-cleanwindowsdevice.md)|None||
|[logoutSharedAppleDeviceActiveUser](../api/manageddevice-logoutsharedappledeviceactiveuser.md)|None||
|[deleteUserFromSharedAppleDevice](../api/manageddevice-deleteuserfromsharedappledevice.md)|None||
|[syncDevice](../api/manageddevice-syncdevice.md)|None||
|[windowsDefenderScan](../api/manageddevice-windowsdefenderscan.md)|None||
|[windowsDefenderUpdateSignatures](../api/manageddevice-windowsdefenderupdatesignatures.md)|None||
|[updateWindowsDeviceAccount](../api/manageddevice-updatewindowsdeviceaccount.md)|None||
|[List deviceConfigurationStates](../api/manageddevice-list-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Get the deviceConfigurationStates from the deviceConfigurationStates navigation property.|
|[Add deviceConfigurationStates](../api/manageddevice-post-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Add deviceConfigurationStates by posting to the deviceConfigurationStates collection.|
|[List deviceCompliancePolicyStates](../api/manageddevice-list-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.|
|[Add deviceCompliancePolicyStates](../api/manageddevice-post-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Add deviceCompliancePolicyStates by posting to the deviceCompliancePolicyStates collection.|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read properties and relationships of the [deviceCategory](../resources/devicecategory.md) object.|
|[List managedDevices](../api/user-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Add managedDevices](../api/user-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Add managedDevices by posting to the managedDevices collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activationLockBypassCode|String|Code that allows the Activation Lock on a device to be bypassed.|
|androidSecurityPatchLevel|String|Android security patch level|
|azureADDeviceId|String|The unique identifier for the Azure Active Directory device. Read only.|
|azureADRegistered|Boolean|Whether the device is Azure Active Directory registered.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|complianceState|Enumeration|Compliance state of the device. Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/configurationmanagerclientenabledfeatures.md)|ConfigrMgr client enabled features|
|deviceActionResults|[deviceActionResult](../resources/deviceactionresult.md) collection|List of ComplexType deviceActionResult objects.|
|deviceCategoryDisplayName|String|Device category display name|
|deviceEnrollmentType|Enumeration|Enrollment type of the device. Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/devicehealthattestationstate.md)|The device health attestation state.|
|deviceName|String|Name of the device|
|deviceRegistrationState|Enumeration|Device registration state. Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|easActivated|Boolean|Whether the device is Exchange ActiveSync activated.|
|easActivationDateTime|DateTimeOffset|Exchange ActivationSync activation time of the device.|
|easDeviceId|String|Exchange ActiveSync Id of the device.|
|emailAddress|String|Email(s) for the user associated with the device|
|enrolledDateTime|DateTimeOffset|Enrollment time of the device.|
|exchangeAccessState|Enumeration|The Access State of the device in Exchange. Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|Enumeration|The reason for the device's access state in Exchange. Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Last time the device contacted Exchange.|
|freeStorageSpaceInBytes|Int64|Free Storage in Bytes|
|id|String| Inherited from [entity](../resources/entity.md)|
|imei|String|IMEI|
|isEncrypted|Boolean|Device encryption status|
|isSupervised|Boolean|Device supervised status|
|jailBroken|String|whether the device is jail broken or rooted.|
|lastSyncDateTime|DateTimeOffset|The date and time that the device last completed a successful sync with Intune.|
|managedDeviceName|String|Automatically generated name to identify a device. Can be overwritten to a user friendly name.|
|managedDeviceOwnerType|Enumeration|Ownership of the device. Can be 'company' or 'personal'. Possible values are: `unknown`, `company`, `personal`.|
|managementAgent|Enumeration|Management channel of the device. Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|manufacturer|String|Manufacturer of the device|
|meid|String|MEID|
|model|String|Model of the device|
|operatingSystem|String|Operating system of the device. Windows, iOS, etc.|
|osVersion|String|Operating system version of the device.|
|partnerReportedThreatState|Enumeration|Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device. Read Only. Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|phoneNumber|String|Phone number of the device|
|remoteAssistanceSessionErrorDetails|String|An error string that identifies issues when creating Remote Assistance session objects.|
|remoteAssistanceSessionUrl|String|Url that allows a Remote Assistance session to be established with the device.|
|serialNumber|String|SerialNumber|
|subscriberCarrier|String|Subscriber Carrier|
|totalStorageSpaceInBytes|Int64|Total Storage in Bytes|
|userDisplayName|String|User display name|
|userId|String|Unique Identifier for the user associated with the device|
|userPrincipalName|String|Device user principal name|
|wiFiMacAddress|String|Wi-Fi MAC|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/devicecategory.md)|Device category|
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Device compliance policy states for this device.|
|deviceConfigurationStates|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Device configuration states for this device.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```

