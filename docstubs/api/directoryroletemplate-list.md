---
title: "List directoryRoleTemplates"
description: "List properties and relationships of the directoryRoleTemplate objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directoryRoleTemplates

Namespace: microsoft.graph

List properties and relationships of the [directoryRoleTemplate](../resources/directoryroletemplate.md) objects.

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
GET /directoryRoleTemplates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryroletemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryRoleTemplate",
      "id": "be40dcf2-dcf2-be40-f2dc-40bef2dc40be",
      "deletedDateTime": "2017-01-01T00:03:00.2666497+00:00",
      "description": "Description value",
      "displayName": "Display Name value"
    }
  ]
}
```

