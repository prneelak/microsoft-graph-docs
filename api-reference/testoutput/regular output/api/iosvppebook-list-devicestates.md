---
title: "List deviceStates"
description: "Get the deviceInstallStates from the deviceStates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceStates

Namespace: microsoft.graph

Get the deviceInstallStates from the deviceStates navigation property.

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
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/deviceinstallstate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceinstallstate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceinstallstate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 492

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceInstallState",
      "id": "387d819e-819e-387d-9e81-7d389e817d38",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2016-12-31T23:59:45.269987+03:00",
      "installState": "String",
      "errorCode": "Error Code value",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value"
    }
  ]
}
```

