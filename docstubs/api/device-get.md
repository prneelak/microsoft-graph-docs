---
title: "Get device"
description: "Read properties and relationships of the device object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get device

Namespace: microsoft.graph

Read properties and relationships of the [device](../resources/device.md) object.

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
GET /devices/{devicesId}
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
If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_device"
}
-->
``` http
GET https://graph.microsoft.com/localtest/devices/{devicesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1242

{
  "value": {
    "@odata.type": "#microsoft.graph.device",
    "id": "f503b0e3-b0e3-f503-e3b0-03f5e3b003f5",
    "deletedDateTime": "2016-12-31T23:57:46.8937102+00:00",
    "accountEnabled": true,
    "alternativeSecurityIds": [
      {
        "@odata.type": "microsoft.graph.alternativeSecurityId",
        "type": 4,
        "identityProvider": "Identity Provider value",
        "key": "a2V5"
      }
    ],
    "approximateLastSignInDateTime": "2017-01-01T00:02:04.9991485+00:00",
    "complianceExpirationDateTime": "2016-12-31T23:58:04.9142646+00:00",
    "deviceId": "Device Id value",
    "deviceMetadata": "Device Metadata value",
    "deviceVersion": 13,
    "displayName": "Display Name value",
    "isCompliant": true,
    "isManaged": true,
    "mdmAppId": "Mdm App Id value",
    "onPremisesLastSyncDateTime": "2016-12-31T23:59:42.0239226+00:00",
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
}
```

