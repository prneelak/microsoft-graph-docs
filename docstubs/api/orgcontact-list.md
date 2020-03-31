---
title: "List orgContacts"
description: "List properties and relationships of the orgContact objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List orgContacts

Namespace: microsoft.graph

List properties and relationships of the [orgContact](../resources/orgcontact.md) objects.

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
GET /contacts
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
If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}
-->
``` http
GET https://graph.microsoft.com/beta/contacts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.orgcontact)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1609

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "70a6ea64-ea64-70a6-64ea-a67064eaa670",
      "deletedDateTime": "2016-12-31T23:59:31.2455853+03:00",
      "addresses": [
        {
          "@odata.type": "microsoft.graph.physicalOfficeAddress",
          "city": "City value",
          "countryOrRegion": "Country Or Region value",
          "officeLocation": "Office Location value",
          "postalCode": "Postal Code value",
          "state": "State value",
          "street": "Street value"
        }
      ],
      "companyName": "Company Name value",
      "department": "Department value",
      "displayName": "Display Name value",
      "givenName": "Given Name value",
      "jobTitle": "Job Title value",
      "mail": "Mail value",
      "mailNickname": "Mail Nickname value",
      "onPremisesSyncEnabled": true,
      "onPremisesLastSyncDateTime": "2016-12-31T23:58:50.4582097+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:58:07.4517849+03:00"
        }
      ],
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone",
          "type": "String",
          "number": "Number value"
        }
      ],
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "surname": "Surname value"
    }
  ]
}
```

