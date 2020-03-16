---
title: "Add columns"
description: "Add columns by posting to the columns collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add columns

Namespace: microsoft.graph

Add columns by posting to the columns collection.

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookTableColumn](../resources/workbooktablecolumn.md) object.

The following table shows the properties that are required when you create the [workbookTableColumn](../resources/workbooktablecolumn.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|name|String||
|values|[Json](../resources/json.md)||



## Response
If successful, this method returns a `201 Created` response code and a [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbooktablecolumn_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.workbookTableColumn",
  "index": 5,
  "name": "Name value",
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
  "@odata.type": "microsoft.graph.workbooktablecolumn"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 214

{
  "@odata.type": "#microsoft.graph.workbookTableColumn",
  "id": "006436a3-36a3-0064-a336-6400a3366400",
  "index": 5,
  "name": "Name value",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

