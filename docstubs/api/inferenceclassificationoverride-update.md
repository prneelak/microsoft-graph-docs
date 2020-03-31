---
title: "Update inferenceClassificationOverride"
description: "Update the properties of a inferenceClassificationOverride object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update inferenceClassificationOverride

Namespace: microsoft.graph

Update the properties of a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.

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
PATCH /me/inferenceClassification/overrides/{inferenceClassificationOverrideId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.

The following table shows the properties that are required when you create the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|classifyAs|Enumeration| Possible values are: `focused`, `other`.|
|senderEmailAddress|[emailAddress](../resources/emailaddress.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/inferenceClassification/overrides/{inferenceClassificationOverrideId}
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
  "classifyAs": "String",
  "senderEmailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
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
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
  "id": "dd7fede0-ede0-dd7f-e0ed-7fdde0ed7fdd",
  "classifyAs": "String",
  "senderEmailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  }
}
```

