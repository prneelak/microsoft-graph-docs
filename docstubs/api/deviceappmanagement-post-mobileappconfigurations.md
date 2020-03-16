---
title: "Add mobileAppConfigurations"
description: "Add mobileAppConfigurations by posting to the mobileAppConfigurations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add mobileAppConfigurations

Namespace: microsoft.graph

Add mobileAppConfigurations by posting to the mobileAppConfigurations collection.

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
POST /deviceAppManagement/mobileAppConfigurations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) object.

The following table shows the properties that are required when you create the [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetedMobileApps|String collection|the associated app.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|displayName|String|Admin provided name of the device configuration.|
|version|Int32|Version of the device configuration.|



## Response
If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_manageddevicemobileappconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 240

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.manageddevicemobileappconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 412

{
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
```

