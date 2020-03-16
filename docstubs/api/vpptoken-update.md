---
title: "Update vppToken"
description: "Update the properties of a vppToken object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update vppToken

Namespace: microsoft.graph

Update the properties of a [vppToken](../resources/vpptoken.md) object.

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
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [vppToken](../resources/vpptoken.md) object.

The following table shows the properties that are required when you create the [vppToken](../resources/vpptoken.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|organizationName|String|The organization associated with the Apple Volume Purchase Program Token|
|vppTokenAccountType|Enumeration|The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. Possible values are: `business`, `education`. Possible values are: `business`, `education`.|
|appleId|String|The apple Id associated with the given Apple Volume Purchase Program Token.|
|expirationDateTime|DateTimeOffset|The expiration date time of the Apple Volume Purchase Program Token.|
|lastSyncDateTime|DateTimeOffset|The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.|
|token|String|The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Last modification date time associated with the Apple Volume Purchase Program Token.|
|state|Enumeration|Current state of the Apple Volume Purchase Program Token. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|lastSyncStatus|Enumeration|Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token. Possible values are: `none`, `inProgress`, `completed`, `failed`. Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Whether or not apps for the VPP token will be automatically updated.|
|countryOrRegion|String|Whether or not apps for the VPP token will be automatically updated.|



## Response
If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/vpptoken.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_vpptoken"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 454

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:17.885665+03:00",
  "lastSyncDateTime": "2017-01-01T00:00:47.2519883+03:00",
  "token": "Token value",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
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
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "7184a092-a092-7184-92a0-847192a08471",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "String",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:17.885665+03:00",
  "lastSyncDateTime": "2017-01-01T00:00:47.2519883+03:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

