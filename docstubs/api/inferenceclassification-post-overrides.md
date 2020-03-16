---
title: "Add overrides"
description: "Add overrides by posting to the overrides collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add overrides

Namespace: microsoft.graph

Add overrides by posting to the overrides collection.

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
POST /me/inferenceClassification/overrides/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.

The following table shows the properties that are required when you create the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|classifyAs|Enumeration|. Possible values are: `focused`, `other`.|
|senderEmailAddress|[emailAddress](../resources/emailaddress.md)||



## Response
If successful, this method returns a `201 Created` response code and a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/inferenceClassification/overrides
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
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceclassificationoverride"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
  "id": "6cf586bc-86bc-6cf5-bc86-f56cbc86f56c",
  "classifyAs": "String",
  "senderEmailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  }
}
```

