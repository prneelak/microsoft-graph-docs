---
title: "Update device"
description: "Update the properties of a device object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update device

Namespace: microsoft.graph

Update the properties of a [device](../resources/device.md) object.

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
PATCH /devices/{devicesId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [device](../resources/device.md) object.

The following table shows the properties that are required when you create the [device](../resources/device.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|accountEnabled|Boolean||
|alternativeSecurityIds|[alternativeSecurityId](../resources/alternativesecurityid.md) collection||
|approximateLastSignInDateTime|DateTimeOffset||
|complianceExpirationDateTime|DateTimeOffset||
|deviceId|String||
|deviceMetadata|String||
|deviceVersion|Int32||
|displayName|String||
|isCompliant|Boolean||
|isManaged|Boolean||
|mdmAppId|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesSyncEnabled|Boolean||
|operatingSystem|String||
|operatingSystemVersion|String||
|physicalIds|String collection||
|profileType|String||
|systemLabels|String collection||
|trustType|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [device](../resources/device.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_device"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/devices/{devicesId}
Content-type: application/json
Content-length: 1108

{
  "@odata.type": "#microsoft.graph.device",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2017-01-01T00:02:22.3204427+03:00",
  "complianceExpirationDateTime": "2016-12-31T23:56:49.4301555+03:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "mdmAppId": "Mdm App Id value",
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "Operating System value",
  "operatingSystemVersion": "Operating System Version value",
  "physicalIds": [
    "Physical Ids value"
  ],
  "profileType": "Profile Type value",
  "systemLabels": [
    "System Labels value"
  ],
  "trustType": "Trust Type value"
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
Content-Length: 1157

{
  "@odata.type": "#microsoft.graph.device",
  "id": "392a2023-2023-392a-2320-2a3923202a39",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2017-01-01T00:02:22.3204427+03:00",
  "complianceExpirationDateTime": "2016-12-31T23:56:49.4301555+03:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "mdmAppId": "Mdm App Id value",
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "Operating System value",
  "operatingSystemVersion": "Operating System Version value",
  "physicalIds": [
    "Physical Ids value"
  ],
  "profileType": "Profile Type value",
  "systemLabels": [
    "System Labels value"
  ],
  "trustType": "Trust Type value"
}
```

