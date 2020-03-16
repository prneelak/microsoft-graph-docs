---
title: "Update certificateBasedAuthConfiguration"
description: "Update the properties of a certificateBasedAuthConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update certificateBasedAuthConfiguration

Namespace: microsoft.graph

Update the properties of a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.

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
PATCH /certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.

The following table shows the properties that are required when you create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|certificateAuthorities|[certificateAuthority](../resources/certificateauthority.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_certificatebasedauthconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
Content-type: application/json
Content-length: 528

{
  "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

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
```

