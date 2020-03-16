---
title: "Update orgContact"
description: "Update the properties of a orgContact object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update orgContact

Namespace: microsoft.graph

Update the properties of a [orgContact](../resources/orgcontact.md) object.

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
PATCH /contacts/{contactsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [orgContact](../resources/orgcontact.md) object.

The following table shows the properties that are required when you create the [orgContact](../resources/orgcontact.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|addresses|[physicalOfficeAddress](../resources/physicalofficeaddress.md) collection||
|companyName|String||
|department|String||
|displayName|String||
|givenName|String||
|jobTitle|String||
|mail|String||
|mailNickname|String||
|onPremisesSyncEnabled|Boolean||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection||
|phones|[phone](../resources/phone.md) collection||
|proxyAddresses|String collection||
|surname|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [orgContact](../resources/orgcontact.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/contacts/{contactsId}
Content-type: application/json
Content-length: 1425

{
  "@odata.type": "#microsoft.graph.orgContact",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:37.8106884+03:00"
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
Content-Length: 1474

{
  "@odata.type": "#microsoft.graph.orgContact",
  "id": "196a396e-396e-196a-6e39-6a196e396a19",
  "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:37.8106884+03:00"
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
```

