---
title: "macOSKerberosSingleSignOnExtension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# macOSKerberosSingleSignOnExtension resource type


Namespace: microsoft.graph




Inherits from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeDirectorySiteCode|String|Gets or sets the Active Directory site. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|blockActiveDirectorySiteAutoDiscovery|Boolean|Enables or disables whether the Kerberos extension can automatically determine its site name. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|blockAutomaticLogin|Boolean|Enables or disables Keychain usage. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|cacheName|String|Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|credentialBundleIdAccessControlList|String collection|Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|domainRealms|String collection|Gets or sets a list of realms for custom domain-realm mapping. Realms are case sensitive. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|domains|String collection|Gets or sets a list of hosts or domain names for which the app extension performs SSO. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|isDefaultRealm|Boolean|When true, this profile's realm will be selected as the default. Necessary if multiple Kerberos-type profiles are configured. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordBlockModification|Boolean|Enables or disables password changes. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordChangeUrl|String|Gets or sets the URL that the user will be sent to when they initiate a password change. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordEnableLocalSync|Boolean|Enables or disables password syncing. This won't affect users logged in with a mobile account on macOS. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordExpirationDays|Int32|Overrides the default password expiration in days. For most domains, this value is calculated automatically. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordExpirationNotificationDays|Int32|Gets or sets the number of days until the user is notified that their password will expire (default is 15). Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordMinimumAgeDays|Int32|Gets or sets the minimum number of days until a user can change their password again. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordMinimumLength|Int32|Gets or sets the minimum length of a password. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordPreviousPasswordBlockCount|Int32|Gets or sets the number of previous passwords to block. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordRequireActiveDirectoryComplexity|Boolean|Enables or disables whether passwords must meet Active Directory's complexity requirements. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|passwordRequirementsDescription|String|Gets or sets a description of the password complexity requirements. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|realm|String|Gets or sets the case-sensitive realm name for this profile. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|requireUserPresence|Boolean|Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|
|userPrincipalName|String|Gets or sets the principle user name to use for this profile. The realm name does not need to be included. Inherited from [kerberosSingleSignOnExtension](../resources/kerberossinglesignonextension.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```

