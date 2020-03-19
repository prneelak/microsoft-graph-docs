---
title: "Get domain"
description: "Read properties and relationships of the domain object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get domain

Namespace: microsoft.graph

Read properties and relationships of the [domain](../resources/domain.md) object.

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
GET /domains/{domainsId}
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
If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domain"
}
-->
``` http
GET https://graph.microsoft.com/localtest/domains/{domainsId}
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
Content-Length: 796

{
  "value": {
    "@odata.type": "#microsoft.graph.domain",
    "id": "198539a6-39a6-1985-a639-8519a6398519",
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
      "@odata.type": "microsoft.graph.domainState",
      "status": "Status value",
      "operation": "Operation value",
      "lastActionDateTime": "2017-01-01T00:00:05.6627106+03:00"
    }
  }
}
```

