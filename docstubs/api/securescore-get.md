---
title: "Get secureScore"
description: "Read properties and relationships of the secureScore object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get secureScore

Namespace: microsoft.graph

Read properties and relationships of the [secureScore](../resources/securescore.md) object.

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
GET /Security/secureScores/{secureScoreId}
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
If successful, this method returns a `200 OK` response code and [secureScore](../resources/securescore.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}
-->
``` http
GET https://graph.microsoft.com/localtest/Security/secureScores/{secureScoreId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScore"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1155

{
  "value": {
    "@odata.type": "#microsoft.graph.secureScore",
    "id": "4542d588-d588-4542-88d5-424588d54245",
    "activeUserCount": 15,
    "averageComparativeScores": [
      {
        "@odata.type": "microsoft.graph.averageComparativeScore",
        "averageScore": "Double",
        "basis": "Basis value"
      }
    ],
    "azureTenantId": "Azure Tenant Id value",
    "controlScores": [
      {
        "@odata.type": "microsoft.graph.controlScore",
        "controlCategory": "Control Category value",
        "controlName": "Control Name value",
        "description": "Description value",
        "score": "Double"
      }
    ],
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "currentScore": "Double",
    "enabledServices": [
      "Enabled Services value"
    ],
    "licensedUserCount": 1,
    "maxScore": "Double",
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation",
      "provider": "Provider value",
      "providerVersion": "Provider Version value",
      "subProvider": "Sub Provider value",
      "vendor": "Vendor value"
    }
  }
}
```

