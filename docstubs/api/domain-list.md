---
title: "List domains"
description: "List properties and relationships of the domain objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List domains

Namespace: microsoft.graph

List properties and relationships of the [domain](../resources/domain.md) objects.

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
GET /domains
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
If successful, this method returns a `200 OK` response code and a collection of [domain](../resources/domain.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domain"
}
-->
``` http
GET https://graph.microsoft.com/localtest/domains
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domain)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "value": [
    {
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
        "@odata.type": "microsoft.graph.domainState",
        "status": "Status value",
        "operation": "Operation value",
        "lastActionDateTime": "2016-12-31T23:56:51.3643763+03:00"
      }
    }
  ]
}
```

