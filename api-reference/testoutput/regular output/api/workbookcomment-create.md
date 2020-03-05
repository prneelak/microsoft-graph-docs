---
title: "Create workbookComment"
description: "Create a new workbookComment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookComment

Namespace: microsoft.graph

Create a new [workbookComment](../resources/workbookcomment.md) object.

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
POST /me/drive/items/{driveItemId}/workbook/comments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookComment](../resources/workbookcomment.md) object.

The following table shows the properties that are required when you create the [workbookComment](../resources/workbookcomment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|String||
|contentType|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookComment](../resources/workbookcomment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookcomment_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/comments
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.workbookComment",
  "content": "Content value",
  "contentType": "Content Type value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookcomment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.workbookComment",
  "id": "a24bf394-f394-a24b-94f3-4ba294f34ba2",
  "content": "Content value",
  "contentType": "Content Type value"
}
```

