---
title: "Get deviceManagement"
description: "Read properties and relationships of the deviceManagement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagement

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagement](../resources/devicemanagement.md) object.

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
GET /deviceManagement
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/devicemanagement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagement"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1420

{
  "value": {
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
}
```

