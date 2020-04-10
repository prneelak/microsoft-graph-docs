---
title: "user: reminderView"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# reminderView

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
GET /me/reminderView
GET /users/{usersId}/reminderView
GET /me/managedDevices/{managedDeviceId}/users/{userId}/reminderView
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|StartDateTime|String||
|EndDateTime|String||



## Response
If successful, this function returns a `200 OK` response code and a [reminder](../resources/reminder.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/reminderView(StartDateTime='parameterValue',EndDateTime='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.reminder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 86

{
  "value": [
    {
      "@odata.type": "microsoft.graph.reminder"
    }
  ]
}
```

