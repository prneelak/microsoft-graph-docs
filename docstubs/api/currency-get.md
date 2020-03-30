---
title: "Get currency"
description: "Read properties and relationships of the currency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get currency

Namespace: microsoft.graph

Read properties and relationships of the [currency](../resources/currency.md) object.

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
GET /financials/companies/{companyId}/currencies/{currencyId}
GET /financials/companies/{companyId}/vendors/{vendorId}/currency
GET /financials/companies/{companyId}/customers/{customerId}/currency
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/currency
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/currency
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/currency
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/currency
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/currency
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
If successful, this method returns a `200 OK` response code and [currency](../resources/currency.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_currency"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/currencies/{currencyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.currency"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 386

{
  "value": {
    "@odata.type": "#microsoft.graph.currency",
    "id": "866fca97-ca97-866f-97ca-6f8697ca6f86",
    "code": "Code value",
    "displayName": "Display Name value",
    "symbol": "Symbol value",
    "amountDecimalPlaces": "Amount Decimal Places value",
    "amountRoundingPrecision": "4.2",
    "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00"
  }
}
```

