---
title: "List schools"
description: "Get the educationSchools from the schools navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List schools

Namespace: microsoft.graph

Get the educationSchools from the schools navigation property.

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
GET /education/classes/{educationClassId}/schools
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/classes/{educationClassId}/schools
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationschool)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1326

{
  "value": [
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
  ]
}
```

