---
title: "List defaultMacOsEnrollmentProfile"
description: "Get the depMacOSEnrollmentProfiles from the defaultMacOsEnrollmentProfile navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List defaultMacOsEnrollmentProfile

Namespace: microsoft.graph

Get the depMacOSEnrollmentProfiles from the defaultMacOsEnrollmentProfile navigation property.

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
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/depmacosenrollmentprofile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_depmacosenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.depmacosenrollmentprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

