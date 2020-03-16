---
title: "Update activityHistoryItem"
description: "Update the properties of a activityHistoryItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update activityHistoryItem

Namespace: microsoft.graph

Update the properties of a [activityHistoryItem](../resources/activityhistoryitem.md) object.

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
PATCH /me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [activityHistoryItem](../resources/activityhistoryitem.md) object.

The following table shows the properties that are required when you create the [activityHistoryItem](../resources/activityhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|activeDurationSeconds|Int32||
|createdDateTime|DateTimeOffset||
|lastActiveDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|startedDateTime|DateTimeOffset||
|userTimezone|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [activityHistoryItem](../resources/activityhistoryitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_activityhistoryitem"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
Content-type: application/json
Content-length: 338

{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "status": "String",
  "activeDurationSeconds": 5,
  "lastActiveDateTime": "2016-12-31T23:59:45.7380499+03:00",
  "expirationDateTime": "2016-12-31T23:57:17.885665+03:00",
  "startedDateTime": "2016-12-31T23:58:31.747746+03:00",
  "userTimezone": "User Timezone value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 510

{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "id": "c662813e-813e-c662-3e81-62c63e8162c6",
  "status": "String",
  "activeDurationSeconds": 5,
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "lastActiveDateTime": "2016-12-31T23:59:45.7380499+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "expirationDateTime": "2016-12-31T23:57:17.885665+03:00",
  "startedDateTime": "2016-12-31T23:58:31.747746+03:00",
  "userTimezone": "User Timezone value"
}
```

