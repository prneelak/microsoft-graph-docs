---
title: "List certificateBasedAuthConfiguration"
description: "Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List certificateBasedAuthConfiguration

Namespace: microsoft.graph

Get the certificateBasedAuthConfigurations from the certificateBasedAuthConfiguration navigation property.

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
GET /organization/{organizationId}/certificateBasedAuthConfiguration
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
If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest/organization/{organizationId}/certificateBasedAuthConfiguration
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.certificatebasedauthconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 662

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
      "id": "0579c20f-c20f-0579-0fc2-79050fc27905",
      "certificateAuthorities": [
        {
          "@odata.type": "microsoft.graph.certificateAuthority",
          "isRootAuthority": true,
          "certificateRevocationListUrl": "https://example.com/certificateRevocationListUrl/",
          "deltaCertificateRevocationListUrl": "https://example.com/deltaCertificateRevocationListUrl/",
          "certificate": "Y2VydGlmaWNhdGU=",
          "issuer": "Issuer value",
          "issuerSki": "Issuer Ski value"
        }
      ]
    }
  ]
}
```

