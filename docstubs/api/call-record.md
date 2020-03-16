---
title: "record"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# record

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
POST /communications/calls/{callId}/record
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|prompts|[prompt](../resources/prompt.md) collection||
|bargeInAllowed|Boolean||
|initialSilenceTimeoutInSeconds|Int32||
|maxSilenceTimeoutInSeconds|Int32||
|maxRecordDurationInSeconds|Int32||
|playBeep|Boolean||
|stopTones|String collection||
|clientContext|String||



## Response
If successful, this action returns a `200 OK` response code and a [recordOperation](../resources/recordoperation.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "call_record"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/calls/{callId}/record

Content-type: application/json
Content-length: 346

{
  "prompts": [
    {
      "@odata.type": "microsoft.graph.mediaPrompt"
    }
  ],
  "bargeInAllowed": true,
  "initialSilenceTimeoutInSeconds": 14,
  "maxSilenceTimeoutInSeconds": 10,
  "maxRecordDurationInSeconds": 10,
  "playBeep": true,
  "stopTones": [
    "Stop Tones value"
  ],
  "clientContext": "Client Context value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordoperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 395

{
  "value": {
    "@odata.type": "#microsoft.graph.recordOperation",
    "id": "221882f7-82f7-2218-f782-1822f7821822",
    "status": "String",
    "clientContext": "Client Context value",
    "resultInfo": {
      "@odata.type": "microsoft.graph.resultInfo"
    },
    "recordingLocation": "Recording Location value",
    "recordingAccessToken": "Recording Access Token value"
  }
}
```

