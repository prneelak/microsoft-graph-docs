---
title: "Update detectedApp"
description: "Update the properties of a detectedApp object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update detectedApp

Namespace: microsoft.graph

Update the properties of a [detectedApp](../resources/detectedapp.md) object.

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
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [detectedApp](../resources/detectedapp.md) object.

The following table shows the properties that are required when you create the [detectedApp](../resources/detectedapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Name of the discovered application. Read-only|
|version|String|Version of the discovered application. Read-only|
|sizeInByte|Int64|Discovered application size in bytes. Read-only|
|deviceCount|Int32|The number of devices that have installed this application|



## Response
If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/detectedapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_detectedapp"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
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
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "5b280f79-0f79-5b28-790f-285b790f285b",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

