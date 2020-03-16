---
title: "Create managedAppRegistrations"
description: "Create managedAppRegistrations by posting to the managedAppRegistrations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create managedAppRegistrations

Namespace: microsoft.graph

Create managedAppRegistrations by posting to the managedAppRegistrations collection.

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
POST /me/managedAppRegistrations/$ref
POST /users/{usersId}/managedAppRegistrations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedAppRegistration](../resources/managedappregistration.md) object.

The following table shows the properties that are required when you create the [managedAppRegistration](../resources/managedappregistration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|Date and time of creation|
|lastSyncDateTime|DateTimeOffset|Date and time of last the app synced with management service.|
|applicationVersion|String|App version|
|managementSdkVersion|String|App management SDK version|
|platformVersion|String|Operating System version|
|deviceType|String|Host device type|
|deviceTag|String|App management SDK generated tag, which helps relate apps hosted on the same device. Not guaranteed to relate apps in all conditions.|
|deviceName|String|Host device name|
|flaggedReasons|Enumeration collection|Zero or more reasons an app registration is flagged. E.g. app running on rooted device. Possible values are: `none`, `rootedDevice`.|
|userId|String|The user Id to who this app registration belongs.|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The app package Identifier|
|version|String|Version of the entity.|



## Response
If successful, this method returns a `201 Created` response code and a [managedAppRegistration](../resources/managedappregistration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedappregistration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/managedAppRegistrations
Content-type: application/json
Content-length: 587

{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedappregistration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 695

{
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
```

