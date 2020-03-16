---
title: "Update deviceCategory"
description: "Update the properties of a deviceCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceCategory

Namespace: microsoft.graph

Update the properties of a [deviceCategory](../resources/devicecategory.md) object.

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
PATCH /me/managedDevices/{managedDeviceId}/deviceCategory
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceCategory](../resources/devicecategory.md) object.

The following table shows the properties that are required when you create the [deviceCategory](../resources/devicecategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name for the device category.|
|description|String|Optional description for the device category.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/devicecategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicecategory"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
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
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "5d55aa3c-aa3c-5d55-3caa-555d3caa555d",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

