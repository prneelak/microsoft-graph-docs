---
title: "List onenoteOperations"
description: "List properties and relationships of the onenoteOperation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onenoteOperations

Namespace: microsoft.graph

List properties and relationships of the [onenoteOperation](../resources/onenoteoperation.md) objects.

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
GET /me/onenote/operations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onenoteOperation](../resources/onenoteoperation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/onenote/operations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onenoteoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onenoteOperation",
      "id": "ca042d37-2d37-ca04-372d-04ca372d04ca",
      "status": "String",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "lastActionDateTime": "2017-01-01T00:03:19.3737597+03:00",
      "resourceLocation": "Resource Location value",
      "resourceId": "Resource Id value",
      "error": {
        "@odata.type": "microsoft.graph.onenoteOperationError",
        "code": "Code value",
        "message": "Message value"
      },
      "percentComplete": "Percent Complete value"
    }
  ]
}
```

