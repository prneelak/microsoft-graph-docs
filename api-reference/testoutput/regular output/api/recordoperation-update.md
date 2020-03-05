---
title: "Update recordOperation"
description: "Update the properties of a recordOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update recordOperation

Namespace: microsoft.graph

Update the properties of a [recordOperation](../resources/recordoperation.md) object.

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
PATCH ** Entity URI for microsoft.graph.recordOperation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [recordOperation](../resources/recordoperation.md) object.

The following table shows the properties that are required when you create the [recordOperation](../resources/recordoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsoperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|clientContext|String| Inherited from [commsOperation](../resources/commsoperation.md)|
|resultInfo|[resultInfo](../resources/resultinfo.md)| Inherited from [commsOperation](../resources/commsoperation.md)|
|recordingLocation|String||
|recordingAccessToken|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [recordOperation](../resources/recordoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_recordoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.recordOperation not found
Content-type: application/json
Content-length: 377

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "recordingLocation": "Recording Location value",
  "recordingAccessToken": "Recording Access Token value"
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
Content-Length: 426

{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "16c6a0eb-a0eb-16c6-eba0-c616eba0c616",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  },
  "recordingLocation": "Recording Location value",
  "recordingAccessToken": "Recording Access Token value"
}
```

