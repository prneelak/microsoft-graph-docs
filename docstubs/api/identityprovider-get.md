---
title: "Get identityProvider"
description: "Read properties and relationships of the identityProvider object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get identityProvider

Namespace: microsoft.graph

Read properties and relationships of the [identityProvider](../resources/identityprovider.md) object.

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
GET /identityProviders/{identityProvidersId}
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
If successful, this method returns a `200 OK` response code and [identityProvider](../resources/identityprovider.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->
``` http
GET https://graph.microsoft.com/localtest/identityProviders/{identityProvidersId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "value": {
    "@odata.type": "#microsoft.graph.identityProvider",
    "id": "e0648eda-8eda-e064-da8e-64e0da8e64e0",
    "type": "Type value",
    "name": "Name value",
    "clientId": "Client Id value",
    "clientSecret": "Client Secret value"
  }
}
```

