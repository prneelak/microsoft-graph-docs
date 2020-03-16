---
title: "Add calendarGroups"
description: "Add calendarGroups by posting to the calendarGroups collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add calendarGroups

Namespace: microsoft.graph

Add calendarGroups by posting to the calendarGroups collection.

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
POST /me/calendarGroups/$ref
POST /users/{usersId}/calendarGroups/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [calendarGroup](../resources/calendargroup.md) object.

The following table shows the properties that are required when you create the [calendarGroup](../resources/calendargroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|classId|Guid||
|changeKey|String||



## Response
If successful, this method returns a `201 Created` response code and a [calendarGroup](../resources/calendargroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/calendarGroups
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "name": "Name value",
  "classId": "faf63209-3209-faf6-0932-f6fa0932f6fa",
  "changeKey": "Change Key value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendargroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 219

{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "id": "d0d1f881-f881-d0d1-81f8-d1d081f8d1d0",
  "name": "Name value",
  "classId": "faf63209-3209-faf6-0932-f6fa0932f6fa",
  "changeKey": "Change Key value"
}
```

