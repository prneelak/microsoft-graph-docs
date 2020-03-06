---
title: "List contracts"
description: "List properties and relationships of the contract objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List contracts

Namespace: microsoft.graph

List properties and relationships of the [contract](../resources/contract.md) objects.

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
GET /contracts
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
If successful, this method returns a `200 OK` response code and a collection of [contract](../resources/contract.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_contract"
}
-->
``` http
GET https://graph.microsoft.com/localtest/contracts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.contract)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contract",
      "id": "55408f20-8f20-5540-208f-4055208f4055",
      "deletedDateTime": "2016-12-31T23:59:54.5724597+03:00",
      "contractType": "Contract Type value",
      "customerId": "870ec555-c555-870e-55c5-0e8755c50e87",
      "defaultDomainName": "Default Domain Name value",
      "displayName": "Display Name value"
    }
  ]
}
```

