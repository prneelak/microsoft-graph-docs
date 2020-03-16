---
title: "Get managedDeviceMobileAppConfiguration"
description: "Read properties and relationships of the managedDeviceMobileAppConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get managedDeviceMobileAppConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) object.

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
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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
If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_manageddevicemobileappconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
    "id": "6f040ebf-0ebf-6f04-bf0e-046fbf0e046f",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```

