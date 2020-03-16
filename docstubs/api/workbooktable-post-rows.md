---
title: "Add rows"
description: "Add rows by posting to the rows collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add rows

Namespace: microsoft.graph

Add rows by posting to the rows collection.

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookTableRow](../resources/workbooktablerow.md) object.

The following table shows the properties that are required when you create the [workbookTableRow](../resources/workbooktablerow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|values|[Json](../resources/json.md)||



## Response
If successful, this method returns a `201 Created` response code and a [workbookTableRow](../resources/workbooktablerow.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbooktablerow_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows
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
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooktablerow"
}
-->
``` http
HTTP/1.1 201 Created
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

