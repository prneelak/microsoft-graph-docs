---
title: "Update contact"
description: "Update the properties of a contact object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update contact

Namespace: microsoft.graph

Update the properties of a [contact](../resources/contact.md) object.

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
PATCH /me/contacts/{contactId}
PATCH /users/{usersId}/contacts/{contactId}
PATCH /me/contactFolders/{contactFolderId}/contacts/{contactId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [contact](../resources/contact.md) object.

The following table shows the properties that are required when you create the [contact](../resources/contact.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|parentFolderId|String||
|birthday|DateTimeOffset||
|fileAs|String||
|displayName|String||
|givenName|String||
|initials|String||
|middleName|String||
|nickName|String||
|surname|String||
|title|String||
|yomiGivenName|String||
|yomiSurname|String||
|yomiCompanyName|String||
|generation|String||
|emailAddresses|[emailAddress](../resources/emailaddress.md) collection||
|imAddresses|String collection||
|jobTitle|String||
|companyName|String||
|department|String||
|officeLocation|String||
|profession|String||
|businessHomePage|String||
|assistantName|String||
|manager|String||
|homePhones|String collection||
|mobilePhone|String||
|businessPhones|String collection||
|homeAddress|[physicalAddress](../resources/physicaladdress.md)||
|businessAddress|[physicalAddress](../resources/physicaladdress.md)||
|otherAddress|[physicalAddress](../resources/physicaladdress.md)||
|spouseName|String||
|personalNotes|String||
|children|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_contact"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/contacts/{contactId}
Content-type: application/json
Content-length: 1902

{
  "@odata.type": "#microsoft.graph.contact",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "parentFolderId": "Parent Folder Id value",
  "birthday": "2016-12-31T23:59:18.574384+03:00",
  "fileAs": "File As value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "initials": "Initials value",
  "middleName": "Middle Name value",
  "nickName": "Nick Name value",
  "surname": "Surname value",
  "title": "Title value",
  "yomiGivenName": "Yomi Given Name value",
  "yomiSurname": "Yomi Surname value",
  "yomiCompanyName": "Yomi Company Name value",
  "generation": "Generation value",
  "emailAddresses": [
    {
      "@odata.type": "microsoft.graph.emailAddress",
      "name": "Name value",
      "address": "Address value"
    }
  ],
  "imAddresses": [
    "Im Addresses value"
  ],
  "jobTitle": "Job Title value",
  "companyName": "Company Name value",
  "department": "Department value",
  "officeLocation": "Office Location value",
  "profession": "Profession value",
  "businessHomePage": "Business Home Page value",
  "assistantName": "Assistant Name value",
  "manager": "Manager value",
  "homePhones": [
    "Home Phones value"
  ],
  "mobilePhone": "Mobile Phone value",
  "businessPhones": [
    "Business Phones value"
  ],
  "homeAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  },
  "businessAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "otherAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "spouseName": "Spouse Name value",
  "personalNotes": "Personal Notes value",
  "children": [
    "Children value"
  ]
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
Content-Length: 2074

{
  "@odata.type": "#microsoft.graph.contact",
  "id": "e06e3dff-3dff-e06e-ff3d-6ee0ff3d6ee0",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "parentFolderId": "Parent Folder Id value",
  "birthday": "2016-12-31T23:59:18.574384+03:00",
  "fileAs": "File As value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "initials": "Initials value",
  "middleName": "Middle Name value",
  "nickName": "Nick Name value",
  "surname": "Surname value",
  "title": "Title value",
  "yomiGivenName": "Yomi Given Name value",
  "yomiSurname": "Yomi Surname value",
  "yomiCompanyName": "Yomi Company Name value",
  "generation": "Generation value",
  "emailAddresses": [
    {
      "@odata.type": "microsoft.graph.emailAddress",
      "name": "Name value",
      "address": "Address value"
    }
  ],
  "imAddresses": [
    "Im Addresses value"
  ],
  "jobTitle": "Job Title value",
  "companyName": "Company Name value",
  "department": "Department value",
  "officeLocation": "Office Location value",
  "profession": "Profession value",
  "businessHomePage": "Business Home Page value",
  "assistantName": "Assistant Name value",
  "manager": "Manager value",
  "homePhones": [
    "Home Phones value"
  ],
  "mobilePhone": "Mobile Phone value",
  "businessPhones": [
    "Business Phones value"
  ],
  "homeAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  },
  "businessAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "otherAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "spouseName": "Spouse Name value",
  "personalNotes": "Personal Notes value",
  "children": [
    "Children value"
  ]
}
```

