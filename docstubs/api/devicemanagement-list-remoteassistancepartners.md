---
title: "List remoteAssistancePartners"
description: "Get the remoteAssistancePartners from the remoteAssistancePartners navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List remoteAssistancePartners

Namespace: microsoft.graph

Get the remoteAssistancePartners from the remoteAssistancePartners navigation property.

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
GET /deviceManagement/remoteAssistancePartners
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
If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/remoteassistancepartner.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_remoteassistancepartner"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/remoteAssistancePartners
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.remoteassistancepartner)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 368

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "46626fe7-6fe7-4662-e76f-6246e76f6246",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "String",
      "lastConnectionDateTime": "2017-01-01T00:03:05.1942522+03:00"
    }
  ]
}
```

