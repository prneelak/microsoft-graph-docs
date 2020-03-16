---
title: "Add operations"
description: "Add operations by posting to the operations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add operations

Namespace: microsoft.graph

Add operations by posting to the operations collection.

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
POST /communications/calls/{callId}/operations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [commsOperation](../resources/commsoperation.md) object.

The following table shows the properties that are required when you create the [commsOperation](../resources/commsoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|clientContext|String||
|resultInfo|[resultInfo](../resources/resultinfo.md)||



## Response
If successful, this method returns a `201 Created` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_commsoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/calls/{callId}/operations
Content-type: application/json
Content-length: 265

{
  "@odata.type": "#microsoft.graph.commsOperation",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.commsoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 314

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "id": "5e712c87-2c87-5e71-872c-715e872c715e",
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

