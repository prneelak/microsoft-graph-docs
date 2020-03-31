---
title: "Add classifyText"
description: "Add classifyText by posting to the classifyText collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add classifyText

Namespace: microsoft.graph

Add classifyText by posting to the classifyText collection.

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
POST /dataClassification/classifyText/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [textClassificationRequest](../resources/textclassificationrequest.md) object.

The following table shows the properties that are required when you create the [textClassificationRequest](../resources/textclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|text|String||
|sensitiveTypeIds|String collection||
|scopesToRun|Enumeration| Possible values are: `fullDocument`, `partialDocument`.|



## Response
If successful, this method returns a `201 Created` response code and a [textClassificationRequest](../resources/textclassificationrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_textclassificationrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/classifyText
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "text": "Text value",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ],
  "scopesToRun": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.textclassificationrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "id": "3a2d6c00-6c00-3a2d-006c-2d3a006c2d3a",
  "text": "Text value",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ],
  "scopesToRun": "String"
}
```

