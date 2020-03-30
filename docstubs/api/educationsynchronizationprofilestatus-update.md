---
title: "Update educationSynchronizationProfileStatus"
description: "Update the properties of a educationSynchronizationProfileStatus object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationSynchronizationProfileStatus

Namespace: microsoft.graph

Update the properties of a [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.

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
PATCH /education/synchronizationProfiles/{educationSynchronizationProfileId}/profileStatus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.

The following table shows the properties that are required when you create the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Possible values are: `paused`, `inProgress`, `success`, `error`, `validationError`, `quarantined`, `unknownFutureValue`.|
|lastSynchronizationDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationsynchronizationprofilestatus"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}/profileStatus
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
  "status": "String",
  "lastSynchronizationDateTime": "2017-01-01T00:00:02.2762663+03:00"
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
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
  "id": "573424cb-24cb-5734-cb24-3457cb243457",
  "status": "String",
  "lastSynchronizationDateTime": "2017-01-01T00:00:02.2762663+03:00"
}
```

