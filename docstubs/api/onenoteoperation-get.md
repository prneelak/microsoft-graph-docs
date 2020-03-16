---
title: "Get onenoteOperation"
description: "Read properties and relationships of the onenoteOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onenoteOperation

Namespace: microsoft.graph

Read properties and relationships of the [onenoteOperation](../resources/onenoteoperation.md) object.

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
GET /me/onenote/operations/{onenoteOperationId}
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
If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/onenote/operations/{onenoteOperationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 572

{
  "value": {
    "@odata.type": "#microsoft.graph.onenoteOperation",
    "id": "e8581b4b-1b4b-e858-4b1b-58e84b1b58e8",
    "status": "String",
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "lastActionDateTime": "2016-12-31T23:56:51.3643763+03:00",
    "resourceLocation": "Resource Location value",
    "resourceId": "Resource Id value",
    "error": {
      "@odata.type": "microsoft.graph.onenoteOperationError",
      "code": "Code value",
      "message": "Message value"
    },
    "percentComplete": "Percent Complete value"
  }
}
```

