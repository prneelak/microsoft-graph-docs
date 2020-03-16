---
title: "Add detectedApps"
description: "Add detectedApps by posting to the detectedApps collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add detectedApps

Namespace: microsoft.graph

Add detectedApps by posting to the detectedApps collection.

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
POST /deviceManagement/detectedApps/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/detectedapp.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_detectedapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/detectedApps
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
  "truncated": true,
  "@odata.type": "microsoft.graph.detectedapp"
}
-->
``` http
HTTP/1.1 201 Created
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

