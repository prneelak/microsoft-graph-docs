---
title: "List directoryRoles"
description: "List properties and relationships of the directoryRole objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directoryRoles

Namespace: microsoft.graph

List properties and relationships of the [directoryRole](../resources/directoryrole.md) objects.

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
GET /directoryRoles
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directoryRole](../resources/directoryrole.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}
-->
``` http
GET https://graph.microsoft.com/localtest/directoryRoles
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
      "id": "2f74a429-a429-2f74-29a4-742f29a4742f",
      "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "roleTemplateId": "Role Template Id value"
    }
  ]
}
```

