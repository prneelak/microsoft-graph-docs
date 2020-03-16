---
title: "List owners"
description: "Get the directoryObjects from the owners navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List owners

Namespace: microsoft.graph

Get the directoryObjects from the owners navigation property.

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
GET /groups/{groupsId}/owners
GET /me/joinedTeams/{groupId}/owners
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
If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/owners
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryobject)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryObject",
      "id": "7f4b5789-5789-7f4b-8957-4b7f89574b7f",
      "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00"
    }
  ]
}
```

