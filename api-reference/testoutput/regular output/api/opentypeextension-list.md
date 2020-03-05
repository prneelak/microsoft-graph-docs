---
title: "List openTypeExtensions"
description: "List properties and relationships of the openTypeExtension objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List openTypeExtensions

Namespace: microsoft.graph

List properties and relationships of the [openTypeExtension](../resources/opentypeextension.md) objects.

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
GET ** Collection URI for microsoft.graph.openTypeExtension not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [openTypeExtension](../resources/opentypeextension.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.openTypeExtension not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.opentypeextension)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 197

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "id": "4db1c125-c125-4db1-25c1-b14d25c1b14d",
      "extensionName": "Extension Name value"
    }
  ]
}
```

