---
title: "Add defaultMacOsEnrollmentProfile"
description: "Add defaultMacOsEnrollmentProfile by posting to the defaultMacOsEnrollmentProfile collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add defaultMacOsEnrollmentProfile

Namespace: microsoft.graph

Add defaultMacOsEnrollmentProfile by posting to the defaultMacOsEnrollmentProfile collection.

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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object.

The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|description|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|configurationEndpointUrl|String|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|**TODO: Add Description** Inherited from [enrollmentProfile](../resources/enrollmentprofile.md)|
|isDefault|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportDepartment|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|passCodeDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|isMandatory|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|restoreBlocked|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|zoomDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|siriDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|deviceNameTemplate|String|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|configurationWebUrl|Boolean|**TODO: Add Description** Inherited from [depEnrollmentBaseProfile](../resources/depenrollmentbaseprofile.md)|
|registrationDisabled|Boolean|**TODO: Add Description**|
|fileVaultDisabled|Boolean|**TODO: Add Description**|
|iCloudDiagnosticsDisabled|Boolean|**TODO: Add Description**|
|iCloudStorageDisabled|Boolean|**TODO: Add Description**|
|chooseYourLockScreenDisabled|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_depmacosenrollmentprofile_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile/$ref
Content-Type: application/json
Content-length: 1270

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": "Boolean",
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": "Boolean",
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean",
  "isDefault": "Boolean",
  "supervisedModeEnabled": "Boolean",
  "supportDepartment": "String",
  "passCodeDisabled": "Boolean",
  "isMandatory": "Boolean",
  "locationDisabled": "Boolean",
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": "Boolean",
  "restoreBlocked": "Boolean",
  "appleIdDisabled": "Boolean",
  "termsAndConditionsDisabled": "Boolean",
  "touchIdDisabled": "Boolean",
  "applePayDisabled": "Boolean",
  "zoomDisabled": "Boolean",
  "siriDisabled": "Boolean",
  "diagnosticsDisabled": "Boolean",
  "displayToneSetupDisabled": "Boolean",
  "privacyPaneDisabled": "Boolean",
  "screenTimeScreenDisabled": "Boolean",
  "deviceNameTemplate": "String",
  "configurationWebUrl": "Boolean",
  "registrationDisabled": "Boolean",
  "fileVaultDisabled": "Boolean",
  "iCloudDiagnosticsDisabled": "Boolean",
  "iCloudStorageDisabled": "Boolean",
  "chooseYourLockScreenDisabled": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.depmacosenrollmentprofile"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "a562f451-f451-a562-51f4-62a551f462a5",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": "Boolean",
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": "Boolean",
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": "Boolean",
  "isDefault": "Boolean",
  "supervisedModeEnabled": "Boolean",
  "supportDepartment": "String",
  "passCodeDisabled": "Boolean",
  "isMandatory": "Boolean",
  "locationDisabled": "Boolean",
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": "Boolean",
  "restoreBlocked": "Boolean",
  "appleIdDisabled": "Boolean",
  "termsAndConditionsDisabled": "Boolean",
  "touchIdDisabled": "Boolean",
  "applePayDisabled": "Boolean",
  "zoomDisabled": "Boolean",
  "siriDisabled": "Boolean",
  "diagnosticsDisabled": "Boolean",
  "displayToneSetupDisabled": "Boolean",
  "privacyPaneDisabled": "Boolean",
  "screenTimeScreenDisabled": "Boolean",
  "deviceNameTemplate": "String",
  "configurationWebUrl": "Boolean",
  "registrationDisabled": "Boolean",
  "fileVaultDisabled": "Boolean",
  "iCloudDiagnosticsDisabled": "Boolean",
  "iCloudStorageDisabled": "Boolean",
  "chooseYourLockScreenDisabled": "Boolean"
}
```

