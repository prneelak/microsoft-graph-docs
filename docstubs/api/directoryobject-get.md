---
title: "Get directoryObject"
description: "Read properties and relationships of the directoryObject object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get directoryObject

Namespace: microsoft.graph

Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.

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
GET /directoryObjects/{directoryObjectsId}
GET /directory/deletedItems/{directoryObjectId}
GET /groups/{groupsId}/acceptedSenders/{directoryObjectId}
GET /groups/{groupsId}/rejectedSenders/{directoryObjectId}
GET /me/joinedTeams/{groupId}/acceptedSenders/{directoryObjectId}
GET /me/joinedTeams/{groupId}/rejectedSenders/{directoryObjectId}
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
If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}
-->
``` http
GET https://graph.microsoft.com/localtest/directoryObjects/{directoryObjectsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
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

