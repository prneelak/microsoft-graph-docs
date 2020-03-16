---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

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
GET /directoryRoles/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [directoryRole](../resources/directoryrole.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "directoryrole_delta"
}
-->
``` http
GET https://graph.microsoft.com/localtest/directoryRoles/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryrole)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryRole",
      "id": "6da244ee-44ee-6da2-ee44-a26dee44a26d",
      "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "roleTemplateId": "Role Template Id value"
    }
  ]
}
```

