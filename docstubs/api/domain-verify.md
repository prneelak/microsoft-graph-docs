---
title: "verify"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# verify

Namespace: microsoft.graph



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
POST /domains/{domainsId}/verify
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [domain](../resources/domain.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}
-->
``` http
POST https://graph.microsoft.com/localtest/domains/{domainsId}/verify
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 658

{
  "value": {
    "@odata.type": "#microsoft.graph.domain",
    "id": "3374b703-b703-3374-03b7-743303b77433",
    "authenticationType": "Authentication Type value",
    "availabilityStatus": "Availability Status value",
    "isAdminManaged": true,
    "isDefault": true,
    "isInitial": true,
    "isRoot": true,
    "isVerified": true,
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "passwordNotificationWindowInDays": 0,
    "passwordValidityPeriodInDays": 12,
    "supportedServices": [
      "Supported Services value"
    ],
    "state": {
      "@odata.type": "microsoft.graph.domainState"
    }
  }
}
```

