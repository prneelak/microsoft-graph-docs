---
title: "Update referenceAttachment"
description: "Update the properties of a referenceAttachment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update referenceAttachment

Namespace: microsoft.graph

Update the properties of a [referenceAttachment](../resources/referenceattachment.md) object.

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
PATCH ** Entity URI for microsoft.graph.referenceAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [referenceAttachment](../resources/referenceattachment.md) object.

The following table shows the properties that are required when you create the [referenceAttachment](../resources/referenceattachment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [attachment](../resources/attachment.md)|
|name|String| Inherited from [attachment](../resources/attachment.md)|
|contentType|String| Inherited from [attachment](../resources/attachment.md)|
|size|Int32| Inherited from [attachment](../resources/attachment.md)|
|isInline|Boolean| Inherited from [attachment](../resources/attachment.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [referenceAttachment](../resources/referenceattachment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_referenceattachment"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.referenceAttachment not found
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true
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
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "6432d743-d743-6432-43d7-326443d73264",
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true
}
```

