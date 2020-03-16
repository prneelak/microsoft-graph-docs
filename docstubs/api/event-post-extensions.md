---
title: "Add extensions"
description: "Add extensions by posting to the extensions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add extensions

Namespace: microsoft.graph

Add extensions by posting to the extensions collection.

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
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/extensions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [extension](../resources/extension.md) object.

The following table shows the properties that are required when you create the [extension](../resources/extension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [extension](../resources/extension.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_extension_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/messages/{messageId}/microsoft.graph.eventMessage/event/extensions
Content-type: application/json
Content-length: 51

{
  "@odata.type": "#microsoft.graph.extension"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extension"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 100

{
  "@odata.type": "#microsoft.graph.extension",
  "id": "8da6bd7b-bd7b-8da6-7bbd-a68d7bbda68d"
}
```

