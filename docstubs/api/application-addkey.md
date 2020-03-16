---
title: "addKey"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# addKey

Namespace: microsoft.graph



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
POST /applications/{applicationsId}/addKey
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|keyCredential|[keyCredential](../resources/keycredential.md)||
|passwordCredential|[passwordCredential](../resources/passwordcredential.md)||
|proof|String||



## Response
If successful, this action returns a `200 OK` response code and a [keyCredential](../resources/keycredential.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "application_addkey"
}
-->
``` http
POST https://graph.microsoft.com/localtest/applications/{applicationsId}/addKey

Content-type: application/json
Content-length: 200

{
  "keyCredential": {
    "@odata.type": "microsoft.graph.keyCredential"
  },
  "passwordCredential": {
    "@odata.type": "microsoft.graph.passwordCredential"
  },
  "proof": "Proof value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keycredential"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 75

{
  "value": {
    "@odata.type": "microsoft.graph.keyCredential"
  }
}
```

