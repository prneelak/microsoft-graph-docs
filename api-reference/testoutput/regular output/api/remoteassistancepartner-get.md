---
title: "Get remoteAssistancePartner"
description: "Read properties and relationships of the remoteAssistancePartner object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get remoteAssistancePartner

Namespace: microsoft.graph

Read properties and relationships of the [remoteAssistancePartner](../resources/remoteassistancepartner.md) object.

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
GET /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
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
If successful, this method returns a `200 OK` response code and [remoteAssistancePartner](../resources/remoteassistancepartner.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_remoteassistancepartner"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.remoteAssistancePartner",
    "id": "4ea84d76-4d76-4ea8-764d-a84e764da84e",
    "displayName": "Display Name value",
    "onboardingUrl": "https://example.com/onboardingUrl/",
    "onboardingStatus": "String",
    "lastConnectionDateTime": "2017-01-01T00:00:23.971855+03:00"
  }
}
```

