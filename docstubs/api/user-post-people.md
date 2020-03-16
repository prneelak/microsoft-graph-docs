---
title: "Add people"
description: "Add people by posting to the people collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add people

Namespace: microsoft.graph

Add people by posting to the people collection.

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
POST /me/people/$ref
POST /users/{usersId}/people/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [person](../resources/person.md) object.

The following table shows the properties that are required when you create the [person](../resources/person.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|givenName|String||
|surname|String||
|birthday|String||
|personNotes|String||
|isFavorite|Boolean||
|scoredEmailAddresses|[scoredEmailAddress](../resources/scoredemailaddress.md) collection||
|phones|[phone](../resources/phone.md) collection||
|postalAddresses|[location](../resources/location.md) collection||
|websites|[website](../resources/website.md) collection||
|jobTitle|String||
|companyName|String||
|yomiCompany|String||
|department|String||
|officeLocation|String||
|profession|String||
|personType|[personType](../resources/persontype.md)||
|userPrincipalName|String||
|imAddress|String||



## Response
If successful, this method returns a `201 Created` response code and a [person](../resources/person.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_person_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/people
Content-type: application/json
Content-length: 2135

{
  "@odata.type": "#microsoft.graph.person",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "surname": "Surname value",
  "birthday": "Birthday value",
  "personNotes": "Person Notes value",
  "isFavorite": true,
  "scoredEmailAddresses": [
    {
      "@odata.type": "microsoft.graph.scoredEmailAddress",
      "address": "Address value",
      "relevanceScore": "Double",
      "selectionLikelihood": "String",
      "itemId": "Item Id value"
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
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location",
      "locationEmailAddress": "Location Email Address value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "locationUri": "Location Uri value",
      "coordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitude": "Double",
        "altitudeAccuracy": "Double"
      },
      "locationType": "String",
      "uniqueId": "Unique Id value",
      "uniqueIdType": "String"
    }
  ],
  "websites": [
    {
      "@odata.type": "microsoft.graph.website",
      "type": "String"
    }
  ],
  "jobTitle": "Job Title value",
  "companyName": "Company Name value",
  "yomiCompany": "Yomi Company value",
  "department": "Department value",
  "officeLocation": "Office Location value",
  "profession": "Profession value",
  "personType": {
    "@odata.type": "microsoft.graph.personType",
    "class": "Class value",
    "subclass": "Subclass value"
  },
  "userPrincipalName": "User Principal Name value",
  "imAddress": "Im Address value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2184

{
  "@odata.type": "#microsoft.graph.person",
  "id": "fa1e27d1-27d1-fa1e-d127-1efad1271efa",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "surname": "Surname value",
  "birthday": "Birthday value",
  "personNotes": "Person Notes value",
  "isFavorite": true,
  "scoredEmailAddresses": [
    {
      "@odata.type": "microsoft.graph.scoredEmailAddress",
      "address": "Address value",
      "relevanceScore": "Double",
      "selectionLikelihood": "String",
      "itemId": "Item Id value"
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
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location",
      "locationEmailAddress": "Location Email Address value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      },
      "locationUri": "Location Uri value",
      "coordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitude": "Double",
        "altitudeAccuracy": "Double"
      },
      "locationType": "String",
      "uniqueId": "Unique Id value",
      "uniqueIdType": "String"
    }
  ],
  "websites": [
    {
      "@odata.type": "microsoft.graph.website",
      "type": "String"
    }
  ],
  "jobTitle": "Job Title value",
  "companyName": "Company Name value",
  "yomiCompany": "Yomi Company value",
  "department": "Department value",
  "officeLocation": "Office Location value",
  "profession": "Profession value",
  "personType": {
    "@odata.type": "microsoft.graph.personType",
    "class": "Class value",
    "subclass": "Subclass value"
  },
  "userPrincipalName": "User Principal Name value",
  "imAddress": "Im Address value"
}
```

