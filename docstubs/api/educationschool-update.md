---
title: "Update educationSchool"
description: "Update the properties of a educationSchool object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationSchool

Namespace: microsoft.graph

Update the properties of a [educationSchool](../resources/educationschool.md) object.

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
PATCH /education/schools/{educationSchoolId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [educationSchool](../resources/educationschool.md) object.

The following table shows the properties that are required when you create the [educationSchool](../resources/educationschool.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [educationOrganization](../resources/educationorganization.md)|
|description|String| Inherited from [educationOrganization](../resources/educationorganization.md)|
|externalSource|Enumeration| Inherited from [educationOrganization](../resources/educationorganization.md). Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail|String||
|principalName|String||
|externalPrincipalId|String||
|lowestGrade|String||
|highestGrade|String||
|schoolNumber|String||
|externalId|String||
|phone|String||
|fax|String||
|createdBy|[identitySet](../resources/identityset.md)||
|address|[physicalAddress](../resources/physicaladdress.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/education/schools/{educationSchoolId}
Content-type: application/json
Content-length: 1104

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "displayName": "Display Name value",
  "description": "Description value",
  "externalSource": "String",
  "principalEmail": "Principal Email value",
  "principalName": "Principal Name value",
  "externalPrincipalId": "External Principal Id value",
  "lowestGrade": "Lowest Grade value",
  "highestGrade": "Highest Grade value",
  "schoolNumber": "School Number value",
  "externalId": "External Id value",
  "phone": "Phone value",
  "fax": "Fax value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  }
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
Content-Length: 1153

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "263b2393-2393-263b-9323-3b2693233b26",
  "displayName": "Display Name value",
  "description": "Description value",
  "externalSource": "String",
  "principalEmail": "Principal Email value",
  "principalName": "Principal Name value",
  "externalPrincipalId": "External Principal Id value",
  "lowestGrade": "Lowest Grade value",
  "highestGrade": "Highest Grade value",
  "schoolNumber": "School Number value",
  "externalId": "External Id value",
  "phone": "Phone value",
  "fax": "Fax value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  }
}
```

