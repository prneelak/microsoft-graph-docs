---
title: "List operations"
description: "Get the managedAppOperations from the operations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List operations

Namespace: microsoft.graph

Get the managedAppOperations from the operations navigation property.

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
GET /me/managedAppRegistrations/{managedAppRegistrationId}/operations
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
If successful, this method returns a `200 OK` response code and a collection of [managedAppOperation](../resources/managedappoperation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managedappoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedappoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppOperation",
      "id": "a683f191-f191-a683-91f1-83a691f183a6",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
      "state": "State value",
      "version": "Version value"
    }
  ]
}
```

