---
title: "Get managedAppRegistration"
description: "Read properties and relationships of the managedAppRegistration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get managedAppRegistration

Namespace: microsoft.graph

Read properties and relationships of the [managedAppRegistration](../resources/managedappregistration.md) object.

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
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
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
If successful, this method returns a `200 OK` response code and [managedAppRegistration](../resources/managedappregistration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managedappregistration"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 750

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppRegistration",
    "id": "d86eb179-b179-d86e-79b1-6ed879b16ed8",
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "lastSyncDateTime": "2017-01-01T00:00:47.2519883+03:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "flaggedReasons": [
      "String"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "version": "Version value"
  }
}
```

