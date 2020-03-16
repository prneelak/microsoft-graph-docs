---
title: "Get calendarGroup"
description: "Read properties and relationships of the calendarGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get calendarGroup

Namespace: microsoft.graph

Read properties and relationships of the [calendarGroup](../resources/calendargroup.md) object.

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
GET /me/calendarGroups/{calendarGroupId}
GET /users/{usersId}/calendarGroups/{calendarGroupId}
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
If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/calendarGroups/{calendarGroupId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": {
    "@odata.type": "#microsoft.graph.calendarGroup",
    "id": "d0d1f881-f881-d0d1-81f8-d1d081f8d1d0",
    "name": "Name value",
    "classId": "faf63209-3209-faf6-0932-f6fa0932f6fa",
    "changeKey": "Change Key value"
  }
}
```

