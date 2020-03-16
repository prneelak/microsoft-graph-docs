---
title: "Update deviceManagement"
description: "Update the properties of a deviceManagement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagement

Namespace: microsoft.graph

Update the properties of a [deviceManagement](../resources/devicemanagement.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagement](../resources/devicemanagement.md) object.

The following table shows the properties that are required when you create the [deviceManagement](../resources/devicemanagement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settings|[deviceManagementSettings](../resources/devicemanagementsettings.md)|Account level settings.|
|intuneBrand|[intuneBrand](../resources/intunebrand.md)|intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.|
|subscriptionState|Enumeration|Tenant mobile device management subscription state. Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/devicemanagement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagement"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement
Content-type: application/json
Content-length: 1278

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "Display Name value",
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  },
  "subscriptionState": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1327

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "dac9e3c9-e3c9-dac9-c9e3-c9dac9e3c9da",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "Display Name value",
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent"
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  },
  "subscriptionState": "String"
}
```

