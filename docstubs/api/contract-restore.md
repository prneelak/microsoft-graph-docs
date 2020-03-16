---
title: "restore"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# restore

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
POST /contracts/{contractsId}/restore
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "contract_restore"
}
-->
``` http
POST https://graph.microsoft.com/localtest/contracts/{contractsId}/restore
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryobject"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 190

{
  "value": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "7f4b5789-5789-7f4b-8957-4b7f89574b7f",
    "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00"
  }
}
```

