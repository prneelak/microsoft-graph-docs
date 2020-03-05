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

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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
GET https://graph.microsoft.com/localtest/contacts
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
Content-Length: 1687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "5077ab57-ab57-5077-57ab-775057ab7750",
      "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
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
      "onPremisesLastSyncDateTime": "2017-01-01T00:03:02.9589742+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:59:30.1342335+03:00"
        }
      ],
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone",
          "type": "String",
          "number": "Number value",
          "region": "Region value",
          "language": "Language value"
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

