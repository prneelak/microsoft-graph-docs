---
title: "Update secureScore"
description: "Update the properties of a secureScore object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update secureScore

Namespace: microsoft.graph

Update the properties of a [secureScore](../resources/securescore.md) object.

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
PATCH /Security/secureScores/{secureScoreId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [secureScore](../resources/securescore.md) object.

The following table shows the properties that are required when you create the [secureScore](../resources/securescore.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activeUserCount|Int32||
|averageComparativeScores|[averageComparativeScore](../resources/averagecomparativescore.md) collection||
|azureTenantId|String||
|controlScores|[controlScore](../resources/controlscore.md) collection||
|createdDateTime|DateTimeOffset||
|currentScore|Double||
|enabledServices|String collection||
|licensedUserCount|Int32||
|maxScore|Double||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [secureScore](../resources/securescore.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_securescore"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Security/secureScores/{secureScoreId}
Content-type: application/json
Content-length: 960

{
  "@odata.type": "#microsoft.graph.secureScore",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1068

{
  "@odata.type": "#microsoft.graph.secureScore",
  "id": "a05d8594-8594-a05d-9485-5da094855da0",
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
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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
```

