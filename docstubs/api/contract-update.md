---
title: "Update contract"
description: "Update the properties of a contract object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update contract

Namespace: microsoft.graph

Update the properties of a [contract](../resources/contract.md) object.

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
PATCH /contracts/{contractsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [contract](../resources/contract.md) object.

The following table shows the properties that are required when you create the [contract](../resources/contract.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|contractType|String||
|customerId|Guid||
|defaultDomainName|String||
|displayName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [contract](../resources/contract.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_contract"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/contracts/{contractsId}
Content-type: application/json
Content-length: 301

{
  "@odata.type": "#microsoft.graph.contract",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "contractType": "Contract Type value",
  "customerId": "f3a93c25-3c25-f3a9-253c-a9f3253ca9f3",
  "defaultDomainName": "Default Domain Name value",
  "displayName": "Display Name value"
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
Content-Length: 350

{
  "@odata.type": "#microsoft.graph.contract",
  "id": "fa096431-6431-fa09-3164-09fa316409fa",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
  "contractType": "Contract Type value",
  "customerId": "f3a93c25-3c25-f3a9-253c-a9f3253ca9f3",
  "defaultDomainName": "Default Domain Name value",
  "displayName": "Display Name value"
}
```

