---
title: "Update security"
description: "Update the properties of a security object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update security

Namespace: microsoft.graph

Update the properties of a [security](../resources/security.md) object.

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
PATCH /Security
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [security](../resources/security.md) object.

The following table shows the properties that are required when you create the [security](../resources/security.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [security](../resources/security.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_security"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/Security
Content-type: application/json
Content-length: 50

{
  "@odata.type": "#microsoft.graph.security"
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
Content-Length: 99

{
  "@odata.type": "#microsoft.graph.security",
  "id": "bed84da3-4da3-bed8-a34d-d8bea34dd8be"
}
```

