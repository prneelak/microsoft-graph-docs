---
title: "List extensions"
description: "Get the extensions from the extensions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List extensions

Namespace: microsoft.graph

Get the extensions from the extensions navigation property.

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
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/extensions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [extension](../resources/extension.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_extension"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/messages/{messageId}/microsoft.graph.eventMessage/event/extensions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.extension)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 141

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.extension",
      "id": "b971efb0-efb0-b971-b0ef-71b9b0ef71b9"
    }
  ]
}
```

