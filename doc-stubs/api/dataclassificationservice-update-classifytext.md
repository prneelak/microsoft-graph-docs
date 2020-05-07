---
title: "Update classifyText"
description: "Update the properties of a classifyText object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update classifyText

Namespace: microsoft.graph

Update the properties of a classifyText object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /dataClassification/classifyText
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [textClassificationRequest](../resources/textclassificationrequest.md) object.

The following table shows the properties that are required when you create the [textClassificationRequest](../resources/textclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|text|String|**TODO: Add Description**|
|fileExtension|String|**TODO: Add Description**|
|sensitiveTypeIds|String collection|**TODO: Add Description**|
|scopesToRun|sensitiveTypeScope|**TODO: Add Description**. Possible values are: `fullDocument`, `partialDocument`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [textClassificationRequest](../resources/textclassificationrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_classifytext"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/classifyText
Content-Type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "text": "String",
  "fileExtension": "String",
  "sensitiveTypeIds": [
    "String"
  ],
  "scopesToRun": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "id": "f2227369-7369-f222-6973-22f2697322f2",
  "text": "String",
  "fileExtension": "String",
  "sensitiveTypeIds": [
    "String"
  ],
  "scopesToRun": "String"
}
```

