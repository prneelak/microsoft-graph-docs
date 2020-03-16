---
title: "redirect"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# redirect

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
POST /communications/calls/{callId}/redirect
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
|targets|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection||
|timeout|Int32||
|callbackUri|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "call_redirect"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/calls/{callId}/redirect

Content-type: application/json
Content-length: 213

{
  "targets": [
    {
      "@odata.type": "microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "Replaces Call Id value"
    }
  ],
  "timeout": 7,
  "callbackUri": "Callback Uri value"
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
HTTP/1.1 204 No Content
```

