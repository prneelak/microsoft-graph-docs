---
title: "Update unmuteParticipantOperation"
description: "Update the properties of a unmuteParticipantOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update unmuteParticipantOperation

Namespace: microsoft.graph

Update the properties of a [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) object.

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
PATCH ** Entity URI for microsoft.graph.unmuteParticipantOperation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) object.

The following table shows the properties that are required when you create the [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsoperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|clientContext|String| Inherited from [commsOperation](../resources/commsoperation.md)|
|resultInfo|[resultInfo](../resources/resultinfo.md)| Inherited from [commsOperation](../resources/commsoperation.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_unmuteparticipantoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.unmuteParticipantOperation not found
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  }
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
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "id": "ddc8c2c5-c2c5-ddc8-c5c2-c8ddc5c2c8dd",
  "status": "String",
  "clientContext": "Client Context value",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": 4,
    "subcode": 7,
    "message": "Message value"
  }
}
```

