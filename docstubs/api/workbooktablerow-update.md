---
title: "Update workbookTableRow"
description: "Update the properties of a workbookTableRow object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookTableRow

Namespace: microsoft.graph

Update the properties of a [workbookTableRow](../resources/workbooktablerow.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows/{workbookTableRowId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookTableRow](../resources/workbooktablerow.md) object.

The following table shows the properties that are required when you create the [workbookTableRow](../resources/workbooktablerow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|values|[Json](../resources/json.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookTableRow](../resources/workbooktablerow.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbooktablerow"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows/{workbookTableRowId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "index": 5,
  "values": {
    "@odata.type": "microsoft.graph.Json"
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
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "id": "6a5a38c3-38c3-6a5a-c338-5a6ac3385a6a",
  "index": 5,
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

