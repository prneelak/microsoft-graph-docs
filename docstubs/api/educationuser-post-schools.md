---
title: "Create schools"
description: "Create schools by posting to the schools collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create schools

Namespace: microsoft.graph

Create schools by posting to the schools collection.

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
POST /education/classes/{educationClassId}/members/{educationUserId}/schools/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [educationSchool](../resources/educationschool.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/{educationUserId}/schools
Content-type: application/json
Content-length: 1174

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
    "type": "String",
    "postOfficeBox": "Post Office Box value",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.educationschool"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1223

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "870dbc20-bc20-870d-20bc-0d8720bc0d87",
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
    "type": "String",
    "postOfficeBox": "Post Office Box value",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  }
}
```

