---
title: "Update workbook"
description: "Update the properties of a workbook object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbook

Namespace: microsoft.graph

Update the properties of a [workbook](../resources/workbook.md) object.

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
PATCH /workbooks/{workbooksId}/workbook
PATCH /me/drive/items/{driveItemId}/workbook
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbook](../resources/workbook.md) object.

The following table shows the properties that are required when you create the [workbook](../resources/workbook.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbook](../resources/workbook.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbook"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/workbooks/{workbooksId}/workbook
Content-type: application/json
Content-length: 50

{
  "@odata.type": "#microsoft.graph.workbook"
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
Content-Length: 99

{
  "@odata.type": "#microsoft.graph.workbook",
  "id": "cac36331-6331-cac3-3163-c3ca3163c3ca"
}
```

