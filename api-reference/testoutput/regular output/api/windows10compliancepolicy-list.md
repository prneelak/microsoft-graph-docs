---
title: "List windows10CompliancePolicies"
description: "List properties and relationships of the windows10CompliancePolicy objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windows10CompliancePolicies

Namespace: microsoft.graph

List properties and relationships of the [windows10CompliancePolicy](../resources/windows10compliancepolicy.md) objects.

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
GET ** Collection URI for microsoft.graph.windows10CompliancePolicy not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/windows10compliancepolicy.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windows10compliancepolicy"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.windows10CompliancePolicy not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windows10compliancepolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1255

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
      "id": "151954f3-54f3-1519-f354-1915f3541915",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordRequiredToUnlockFromIdle": true,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "String",
      "passwordPreviousPasswordBlockCount": 2,
      "requireHealthyDeviceReport": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
      "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true
    }
  ]
}
```

