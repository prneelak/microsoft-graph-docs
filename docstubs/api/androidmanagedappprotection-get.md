---
title: "Get androidManagedAppProtection"
description: "Read properties and relationships of the androidManagedAppProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get androidManagedAppProtection

Namespace: microsoft.graph

Read properties and relationships of the [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object.

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
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
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
If successful, this method returns a `200 OK` response code and [androidManagedAppProtection](../resources/androidmanagedappprotection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_androidmanagedappprotection"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidManagedAppProtection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1924

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppProtection",
    "id": "4a122809-2809-4a12-0928-124a0928124a",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
    "version": "Version value",
    "periodOfflineBeforeAccessCheck": "PT58.5444332S",
    "periodOnlineBeforeAccessCheck": "PT2M31.6474097S",
    "allowedInboundDataTransferSources": "String",
    "allowedOutboundDataTransferDestinations": "String",
    "organizationalCredentialsRequired": true,
    "allowedOutboundClipboardSharingLevel": "String",
    "dataBackupBlocked": true,
    "deviceComplianceRequired": true,
    "managedBrowserToOpenLinksRequired": true,
    "saveAsBlocked": true,
    "periodOfflineBeforeWipeIsEnforced": "-PT1M54.3737102S",
    "pinRequired": true,
    "maximumPinRetries": 1,
    "simplePinBlocked": true,
    "minimumPinLength": 0,
    "pinCharacterSet": "String",
    "periodBeforePinReset": "-PT2M11.0428878S",
    "allowedDataStorageLocations": [
      "String"
    ],
    "contactSyncBlocked": true,
    "printBlocked": true,
    "fingerprintBlocked": true,
    "disableAppPinIfDevicePinIsSet": true,
    "minimumRequiredOsVersion": "Minimum Required Os Version value",
    "minimumWarningOsVersion": "Minimum Warning Os Version value",
    "minimumRequiredAppVersion": "Minimum Required App Version value",
    "minimumWarningAppVersion": "Minimum Warning App Version value",
    "isAssigned": true,
    "screenCaptureBlocked": true,
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
    "encryptAppData": true,
    "deployedAppCount": 0,
    "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
    "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
  }
}
```

