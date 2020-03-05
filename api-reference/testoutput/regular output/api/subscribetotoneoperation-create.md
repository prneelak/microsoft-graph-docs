---
title: "Create subscribeToToneOperation"
description: "Create a new subscribeToToneOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create subscribeToToneOperation

Namespace: microsoft.graph

Create a new [subscribeToToneOperation](../resources/subscribetotoneoperation.md) object.

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
POST ** Collection URI for microsoft.graph.subscribeToToneOperation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [subscribeToToneOperation](../resources/subscribetotoneoperation.md) object.

The following table shows the properties that are required when you create the [subscribeToToneOperation](../resources/subscribetotoneoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsoperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|clientContext|String| Inherited from [commsOperation](../resources/commsoperation.md)|
|resultInfo|[resultInfo](../resources/resultinfo.md)| Inherited from [commsOperation](../resources/commsoperation.md)|



## Response
If successful, this method returns a `201 Created` response code and a [subscribeToToneOperation](../resources/subscribetotoneoperation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_subscribetotoneoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.subscribeToToneOperation not found
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
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
  "@odata.type": "microsoft.graph.subscribetotoneoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "id": "db13e723-e723-db13-23e7-13db23e713db",
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

