---
title: "managedDevice: getFileVaultKey"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getFileVaultKey

Namespace: microsoft.graph



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
GET /me/managedDevices/{managedDeviceId}/getFileVaultKey
GET /users/{usersId}/managedDevices/{managedDeviceId}/getFileVaultKey
GET /deviceManagement/managedDevices/{managedDeviceId}/getFileVaultKey
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a String in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "manageddevice_getfilevaultkey"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/getFileVaultKey
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "edm.string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 43

{
  "value": "Get File Vault Key value"
}
```

