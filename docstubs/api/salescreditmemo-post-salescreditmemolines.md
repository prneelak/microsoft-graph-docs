---
title: "Add salesCreditMemoLines"
description: "Add salesCreditMemoLines by posting to the salesCreditMemoLines collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add salesCreditMemoLines

Namespace: microsoft.graph

Add salesCreditMemoLines by posting to the salesCreditMemoLines collection.

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
POST /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [salesCreditMemoLine](../resources/salescreditmemoline.md) object.

The following table shows the properties that are required when you create the [salesCreditMemoLine](../resources/salescreditmemoline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|documentId|Guid||
|sequence|Int32||
|itemId|Guid||
|accountId|Guid||
|lineType|String||
|description|String||
|unitOfMeasureId|Guid||
|unitPrice|Decimal||
|quantity|Decimal||
|discountAmount|Decimal||
|discountPercent|Decimal||
|discountAppliedBeforeTax|Boolean||
|amountExcludingTax|Decimal||
|taxCode|String||
|taxPercent|Decimal||
|totalTaxAmount|Decimal||
|amountIncludingTax|Decimal||
|invoiceDiscountAllocation|Decimal||
|netAmount|Decimal||
|netTaxAmount|Decimal||
|netAmountIncludingTax|Decimal||
|shipmentDate|Date||



## Response
If successful, this method returns a `201 Created` response code and a [salesCreditMemoLine](../resources/salescreditmemoline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_salescreditmemoline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines
Content-type: application/json
Content-length: 817

{
  "@odata.type": "#microsoft.graph.salesCreditMemoLine",
  "documentId": "ad0679c0-79c0-ad06-c079-06adc07906ad",
  "sequence": 8,
  "itemId": "b63d2521-2521-b63d-2125-3db621253db6",
  "accountId": "93d19a1f-9a1f-93d1-1f9a-d1931f9ad193",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "e854acc8-acc8-e854-c8ac-54e8c8ac54e8",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salescreditmemoline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 866

{
  "@odata.type": "#microsoft.graph.salesCreditMemoLine",
  "id": "73f000be-00be-73f0-be00-f073be00f073",
  "documentId": "ad0679c0-79c0-ad06-c079-06adc07906ad",
  "sequence": 8,
  "itemId": "b63d2521-2521-b63d-2125-3db621253db6",
  "accountId": "93d19a1f-9a1f-93d1-1f9a-d1931f9ad193",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "e854acc8-acc8-e854-c8ac-54e8c8ac54e8",
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
```

