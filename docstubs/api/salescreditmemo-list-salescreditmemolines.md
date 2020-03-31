---
title: "List salesCreditMemoLines"
description: "Get the salesCreditMemoLines from the salesCreditMemoLines navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesCreditMemoLines

Namespace: microsoft.graph

Get the salesCreditMemoLines from the salesCreditMemoLines navigation property.

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
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines
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
If successful, this method returns a `200 OK` response code and a collection of [salesCreditMemoLine](../resources/salescreditmemoline.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemoline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salescreditmemoline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 995

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesCreditMemoLine",
      "id": "41098071-8071-4109-7180-094171800941",
      "documentId": "80f7ddfe-ddfe-80f7-fedd-f780feddf780",
      "sequence": 8,
      "itemId": "5e7338b8-38b8-5e73-b838-735eb838735e",
      "accountId": "ca9f694c-694c-ca9f-4c69-9fca4c699fca",
      "lineType": "Line Type value",
      "description": "Description value",
      "unitOfMeasureId": "edff6ece-6ece-edff-ce6e-ffedce6effed",
      "unitPrice": "4.2",
      "quantity": "4.2",
      "discountAmount": "4.2",
      "discountPercent": "4.2",
      "discountAppliedBeforeTax": true,
      "amountExcludingTax": "4.2",
      "taxCode": "Tax Code value",
      "taxPercent": "4.2",
      "totalTaxAmount": "4.2",
      "amountIncludingTax": "4.2",
      "invoiceDiscountAllocation": "4.2",
      "netAmount": "4.2",
      "netTaxAmount": "4.2",
      "netAmountIncludingTax": "4.2",
      "shipmentDate": "Date"
    }
  ]
}
```

