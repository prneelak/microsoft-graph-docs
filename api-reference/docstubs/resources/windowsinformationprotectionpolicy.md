---
title: "windowsInformationProtectionPolicy resource type"
description: "Policy for Windows information protection without MDM"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtectionPolicy resource type


Namespace: microsoft.graph

Policy for Windows information protection without MDM


Inherits from [windowsInformationProtection](../resources/windowsinformationprotection.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionPolicy](../api/windowsinformationprotectionpolicy-get.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md)|Read the properties and relationships of a [windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) object.|
|[Update windowsInformationProtectionPolicy](../api/windowsinformationprotectionpolicy-update.md)|[windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md)|Update the properties of a [windowsInformationProtectionPolicy](../resources/windowsinformationprotectionpolicy.md) object.|
|[assign](../api/windowsinformationprotectionpolicy-assign.md)|None|**TODO: Add Description**|
|[List protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-list-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the protectedAppLockerFiles navigation property.|
|[Create protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-post-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Create a new protectedAppLockerFiles object.|
|[Delete protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-delete-protectedapplockerfiles.md)|None|Delete a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[Update protectedAppLockerFiles](../api/windowsinformationprotectionpolicy-update-protectedapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Update the properties of a protectedAppLockerFiles object.|
|[Get windowsInformationProtectionAppLockerFile](../api/windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[List exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-list-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Get the windowsInformationProtectionAppLockerFiles from the exemptAppLockerFiles navigation property.|
|[Create exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-post-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Create a new exemptAppLockerFiles object.|
|[Delete exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-delete-exemptapplockerfiles.md)|None|Delete an [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[Update exemptAppLockerFiles](../api/windowsinformationprotectionpolicy-update-exemptapplockerfiles.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Update the properties of an exemptAppLockerFiles object.|
|[Get windowsInformationProtectionAppLockerFile](../api/windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Read the properties and relationships of a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[List assignments](../api/windowsinformationprotectionpolicy-list-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Get the targetedManagedAppPolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsinformationprotectionpolicy-post-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsinformationprotectionpolicy-delete-assignments.md)|None|Delete an [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|
|[Update assignments](../api/windowsinformationprotectionpolicy-update-assignments.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Update the properties of an assignments object.|
|[Get targetedManagedAppPolicyAssignment](../api/targetedmanagedapppolicyassignment-get.md)|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md)|Read the properties and relationships of a [targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|azureRightsManagementServicesAllowed|Boolean|Specifies whether to allow Azure RMS encryption for WIP Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|createdDateTime|DateTimeOffset|The date and time the policy was created. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/windowsinformationprotectiondatarecoverycertificate.md)|Specifies a recovery certificate that can be used for data recovery of encrypted files. This is the same as the data recovery agent(DRA) certificate for encrypting file system(EFS) Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|daysWithoutContactBeforeUnenroll|Int32|Offline interval before app data is wiped (days) |
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|enforcementLevel|windowsInformationProtectionEnforcementLevel|WIP enforcement level.See the Enum definition for supported values Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md). Possible values are: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String|Primary enterprise domain Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|This is the comma-separated list of internal proxy servers. For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59". These proxies have been configured by the admin to connect to specific resources on the Internet. They are considered to be enterprise network locations. The proxies are only leveraged in configuring the EnterpriseProxiedDomains policy to force traffic to the matched domains through these proxies Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/windowsinformationprotectioniprangecollection.md) collection|Sets the enterprise IP ranges that define the computers in the enterprise network. Data that comes from those computers will be considered part of the enterprise and protected. These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseIPRangesAreAuthoritative|Boolean|Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets. Default is false Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|This is the list of domains that comprise the boundaries of the enterprise. Data from one of these domains that is sent to a device will be considered enterprise data and protected These locations will be considered a safe destination for enterprise data to be shared to Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|List of enterprise domains to be protected Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/windowsinformationprotectionproxieddomaincollection.md) collection|Contains a list of Enterprise resource domains hosted in the cloud that need to be protected. Connections to these resources are considered enterprise data. If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80). A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|This is a list of proxy servers. Any server not on this list is considered non-enterprise Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|enterpriseProxyServersAreAuthoritative|Boolean|Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies. Default is false Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|Exempt applications can also access enterprise data, but the data handled by those applications are not protected. This is because some critical enterprise applications may have compatibility problems with encrypted data. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|iconsVisible|Boolean|Determines whether overlays are added to icons for WIP protected files in Explorer and enterprise only app tiles in the Start menu. Starting in Windows 10, version 1703 this setting also configures the visibility of the WIP icon in the title bar of a WIP-protected app Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|indexingEncryptedStoresOrItemsBlocked|Boolean|This switch is for the Windows Search Indexer, to allow or disallow indexing of items Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|isAssigned|Boolean|Indicates if the policy is deployed to any inclusion groups or not. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|mdmEnrollmentUrl|String|Enrollment url for the MDM|
|minutesOfInactivityBeforeDeviceLock|Int32|Specifies the maximum amount of time (in minutes) allowed after the device is idle that will cause the device to become PIN or password locked.   Range is an integer X where 0 <= X <= 999.|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|List of domain names that can used for work or personal resource Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|numberOfPastPinsRemembered|Int32|Integer value that specifies the number of past PINs that can be associated to a user account that can't be reused. The largest number you can configure for this policy setting is 50. The lowest number you can configure for this policy setting is 0. If this policy is set to 0, then storage of previous PINs is not required. This node was added in Windows 10, version 1511. Default is 0.|
|passwordMaximumAttemptCount|Int32|The number of authentication failures allowed before the device will be wiped. A value of 0 disables device wipe functionality. Range is an integer X where 4 <= X <= 16 for desktop and 0 <= X <= 999 for mobile devices.|
|pinExpirationDays|Int32|Integer value specifies the period of time (in days) that a PIN can be used before the system requires the user to change it. The largest number you can configure for this policy setting is 730. The lowest number you can configure for this policy setting is 0. If this policy is set to 0, then the user's PIN will never expire. This node was added in Windows 10, version 1511. Default is 0.|
|pinLowercaseLetters|windowsInformationProtectionPinCharacterRequirements|Integer value that configures the use of lowercase letters in the Windows Hello for Business PIN. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinMinimumLength|Int32|Integer value that sets the minimum number of characters required for the PIN. Default value is 4. The lowest number you can configure for this policy setting is 4. The largest number you can configure must be less than the number configured in the Maximum PIN length policy setting or the number 127, whichever is the lowest.|
|pinSpecialCharacters|windowsInformationProtectionPinCharacterRequirements|Integer value that configures the use of special characters in the Windows Hello for Business PIN. Valid special characters for Windows Hello for Business PIN gestures include: ! " # $ % & ' ( ) * + , - . / : ; < = > ? @ \[ \ \] ^ _ ` { | } ~. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinUppercaseLetters|windowsInformationProtectionPinCharacterRequirements|Integer value that configures the use of uppercase letters in the Windows Hello for Business PIN. Default is NotAllow. Possible values are: `notAllow`, `requireAtLeastOne`, `allow`.|
|protectedApps|[windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md) collection|Protected applications can access enterprise data and the data handled by those applications are protected with encryption Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectionUnderLockConfigRequired|Boolean|Specifies whether the protection under lock feature (also known as encrypt under pin) should be configured Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|revokeOnMdmHandoffDisabled|Boolean|New property in RS2, pending documentation|
|revokeOnUnenrollDisabled|Boolean|This policy controls whether to revoke the WIP keys when a device unenrolls from the management service. If set to 1 (Don't revoke keys), the keys will not be revoked and the user will continue to have access to protected files after unenrollment. If the keys are not revoked, there will be no revoked file cleanup subsequently. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|rightsManagementServicesTemplateId|Guid|TemplateID GUID to use for RMS encryption. The RMS template allows the IT admin to configure the details about who has access to RMS-protected file and how long they have access Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/windowsinformationprotectionresourcecollection.md) collection|Specifies a list of file extensions, so that files with these extensions are encrypted when copying from an SMB share within the corporate boundary Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|version|String|Version of the entity. Inherited from [managedAppPolicy](../resources/managedapppolicy.md)|
|windowsHelloForBusinessBlocked|Boolean|Boolean value that sets Windows Hello for Business as a method for signing into Windows.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[targetedManagedAppPolicyAssignment](../resources/targetedmanagedapppolicyassignment.md) collection|Navigation property to list of security groups targeted for policy. Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Another way to input exempt apps through xml files Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) collection|Another way to input protected apps through xml files Inherited from [windowsInformationProtection](../resources/windowsinformationprotection.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionPolicy",
  "baseType": "microsoft.graph.windowsInformationProtection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv4CidrRange",
          "cidrAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 1024,
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": 1024,
  "numberOfPastPinsRemembered": 1024,
  "passwordMaximumAttemptCount": 1024,
  "minutesOfInactivityBeforeDeviceLock": 1024,
  "daysWithoutContactBeforeUnenroll": 1024
}
```

