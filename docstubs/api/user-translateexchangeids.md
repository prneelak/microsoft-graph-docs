---
title: "user: translateExchangeIds"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# translateExchangeIds

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/translateExchangeIds
POST /users/{usersId}/translateExchangeIds
POST /me/managedDevices/{managedDeviceId}/users/{userId}/translateExchangeIds
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|InputIds|String collection||
|TargetIdType|Enumeration||
|SourceIdType|Enumeration||



## Response
If successful, this action returns a `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

Content-type: application/json
Content-length: 107

{
  "InputIds": [
    "Input Ids value"
  ],
  "TargetIdType": "String",
  "SourceIdType": "String"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.convertidresult)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 93

{
  "value": [
    {
      "@odata.type": "microsoft.graph.convertIdResult"
    }
  ]
}
```

