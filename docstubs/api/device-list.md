---
title: "List devices"
description: "List properties and relationships of the device objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List devices

Namespace: microsoft.graph

List properties and relationships of the [device](../resources/device.md) objects.

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
GET /devices
GET /me/devices
GET /users/{usersId}/devices
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [device](../resources/device.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_device"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.device)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.device",
      "id": "7c1c12ad-12ad-7c1c-ad12-1c7cad121c7c",
      "deletedDateTime": "2016-12-31T23:56:41.707717+03:00",
      "accountEnabled": true,
      "alternativeSecurityIds": [
        {
          "@odata.type": "microsoft.graph.alternativeSecurityId",
          "type": 4,
          "identityProvider": "Identity Provider value",
          "key": "a2V5"
        }
      ],
      "approximateLastSignInDateTime": "2017-01-01T00:01:23.0679402+03:00",
      "complianceExpirationDateTime": "2016-12-31T23:59:57.1462234+03:00",
      "deviceId": "Device Id value",
      "deviceMetadata": "Device Metadata value",
      "deviceVersion": 13,
      "displayName": "Display Name value",
      "isCompliant": true,
      "isManaged": true,
      "onPremisesLastSyncDateTime": "2017-01-01T00:03:26.0023027+03:00",
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
      "trustType": "Trust Type value",
      "Name": "Name value",
      "Manufacturer": "Manufacturer value",
      "Model": "Model value",
      "Kind": "Kind value",
      "Status": "Status value",
      "Platform": "Platform value"
    }
  ]
}
```

