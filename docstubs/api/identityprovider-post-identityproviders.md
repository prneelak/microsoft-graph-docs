---
title: "Create identityProvider"
description: "Create a new identityProvider object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create identityProvider

Namespace: microsoft.graph

Create a new [identityProvider](../resources/identityprovider.md) object.

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
POST /identityProviders
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [identityProvider](../resources/identityprovider.md) object.

The following table shows the properties that are required when you create the [identityProvider](../resources/identityprovider.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String||
|name|String||
|clientId|String||
|clientSecret|String||



## Response
If successful, this method returns a `201 Created` response code and a [identityProvider](../resources/identityprovider.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->
``` http
POST https://graph.microsoft.com/localtest/identityProviders
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.identityProvider",
  "type": "Type value",
  "name": "Name value",
  "clientId": "Client Id value",
  "clientSecret": "Client Secret value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityprovider"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.identityProvider",
  "id": "e0648eda-8eda-e064-da8e-64e0da8e64e0",
  "type": "Type value",
  "name": "Name value",
  "clientId": "Client Id value",
  "clientSecret": "Client Secret value"
}
```

