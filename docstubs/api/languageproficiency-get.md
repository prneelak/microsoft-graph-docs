---
title: "Get languageProficiency"
description: "Read properties and relationships of the languageProficiency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get languageProficiency

Namespace: microsoft.graph

Read properties and relationships of the [languageProficiency](../resources/languageproficiency.md) object.

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
GET /me/profile/languages/{languageProficiencyId}
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
If successful, this method returns a `200 OK` response code and [languageProficiency](../resources/languageproficiency.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_languageproficiency"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/languages/{languageProficiencyId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1031

{
  "value": {
    "@odata.type": "#microsoft.graph.languageProficiency",
    "id": "73537c61-7c61-7353-617c-5373617c5373",
    "allowedAudiences": "String",
    "inference": {
      "@odata.type": "microsoft.graph.inferenceData",
      "confidenceScore": "Double",
      "userHasVerifiedAccuracy": true
    },
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "displayName": "Display Name value",
    "tag": "Tag value",
    "proficiency": "String"
  }
}
```

