---
title: "Get personWebsite"
description: "Read properties and relationships of the personWebsite object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get personWebsite

Namespace: microsoft.graph

Read properties and relationships of the [personWebsite](../resources/personwebsite.md) object.

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
GET /me/profile/websites/{personWebsiteId}
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
If successful, this method returns a `200 OK` response code and [personWebsite](../resources/personwebsite.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_personwebsite"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/websites/{personWebsiteId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1112

{
  "value": {
    "@odata.type": "#microsoft.graph.personWebsite",
    "id": "3a77b16a-b16a-3a77-6ab1-773a6ab1773a",
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
    "categories": [
      "Categories value"
    ],
    "description": "Description value",
    "displayName": "Display Name value",
    "webUrl": "https://example.com/webUrl/"
  }
}
```

