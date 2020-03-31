---
title: "Get certificateBasedAuthConfiguration"
description: "Read properties and relationships of the certificateBasedAuthConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get certificateBasedAuthConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.

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
GET /certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
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
If successful, this method returns a `200 OK` response code and [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "value": {
    "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
    "id": "c6e8d389-d389-c6e8-89d3-e8c689d3e8c6",
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
}
```

