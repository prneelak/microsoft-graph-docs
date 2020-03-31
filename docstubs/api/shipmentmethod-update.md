---
title: "Update shipmentMethod"
description: "Update the properties of a shipmentMethod object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update shipmentMethod

Namespace: microsoft.graph

Update the properties of a [shipmentMethod](../resources/shipmentmethod.md) object.

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
PATCH /financials/companies/{companyId}/shipmentMethods/{shipmentMethodId}
PATCH /financials/companies/{companyId}/customers/{customerId}/shipmentMethod
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/shipmentMethod
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/shipmentMethod
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [shipmentMethod](../resources/shipmentmethod.md) object.

The following table shows the properties that are required when you create the [shipmentMethod](../resources/shipmentmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [shipmentMethod](../resources/shipmentmethod.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_shipmentmethod"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/shipmentMethods/{shipmentMethodId}
Content-type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.shipmentMethod",
  "code": "Code value",
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
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.shipmentMethod",
  "id": "233e81a3-81a3-233e-a381-3e23a3813e23",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

