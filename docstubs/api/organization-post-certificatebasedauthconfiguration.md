---
title: "Create certificateBasedAuthConfiguration"
description: "Create certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create certificateBasedAuthConfiguration

Namespace: microsoft.graph

Create certificateBasedAuthConfiguration by posting to the certificateBasedAuthConfiguration collection.

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
POST /organization/{organizationId}/certificateBasedAuthConfiguration/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.

The following table shows the properties that are required when you create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|certificateAuthorities|[certificateAuthority](../resources/certificateauthority.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}
-->
``` http
POST https://graph.microsoft.com/localtest/organization/{organizationId}/certificateBasedAuthConfiguration
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
  "truncated": true,
  "@odata.type": "microsoft.graph.certificatebasedauthconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
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

