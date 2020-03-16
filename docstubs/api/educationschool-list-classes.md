---
title: "List classes"
description: "Get the educationClasses from the classes navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List classes

Namespace: microsoft.graph

Get the educationClasses from the classes navigation property.

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
GET /education/classes/{educationClassId}/schools/{educationSchoolId}/classes
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
If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/classes/{educationClassId}/schools/{educationSchoolId}/classes
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationclass)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 959

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "9457bab8-bab8-9457-b8ba-5794b8ba5794",
      "displayName": "Display Name value",
      "mailNickname": "Mail Nickname value",
      "description": "Description value",
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
      "classCode": "Class Code value",
      "externalName": "External Name value",
      "externalId": "External Id value",
      "externalSource": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm",
        "startDate": "Date",
        "endDate": "Date"
      }
    }
  ]
}
```

