---
title: "Update journalLine"
description: "Update the properties of a journalLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update journalLine

Namespace: microsoft.graph

Update the properties of a [journalLine](../resources/journalline.md) object.

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
PATCH /financials/companies/{companyId}/journalLines/{journalLineId}
PATCH /financials/companies/{companyId}/journals/{journalId}/journalLines/{journalLineId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [journalLine](../resources/journalline.md) object.

The following table shows the properties that are required when you create the [journalLine](../resources/journalline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String||
|lineNumber|Int32||
|accountId|Guid||
|accountNumber|String||
|postingDate|Date||
|documentNumber|String||
|externalDocumentNumber|String||
|amount|Decimal||
|description|String||
|comment|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [journalLine](../resources/journalline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_journalline"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/journalLines/{journalLineId}
Content-type: application/json
Content-length: 454

{
  "@odata.type": "#microsoft.graph.journalLine",
  "journalDisplayName": "Journal Display Name value",
  "lineNumber": 10,
  "accountId": "16975858-5858-1697-5858-971658589716",
  "accountNumber": "Account Number value",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "externalDocumentNumber": "External Document Number value",
  "amount": "4.2",
  "description": "Description value",
  "comment": "Comment value"
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
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.journalLine",
  "id": "f2d18712-8712-f2d1-1287-d1f21287d1f2",
  "journalDisplayName": "Journal Display Name value",
  "lineNumber": 10,
  "accountId": "16975858-5858-1697-5858-971658589716",
  "accountNumber": "Account Number value",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "externalDocumentNumber": "External Document Number value",
  "amount": "4.2",
  "description": "Description value",
  "comment": "Comment value",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
}
```

