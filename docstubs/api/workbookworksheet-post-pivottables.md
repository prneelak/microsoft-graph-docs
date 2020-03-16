---
title: "Add pivotTables"
description: "Add pivotTables by posting to the pivotTables collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add pivotTables

Namespace: microsoft.graph

Add pivotTables by posting to the pivotTables collection.

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
POST /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/pivotTables/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookPivotTable](../resources/workbookpivottable.md) object.

The following table shows the properties that are required when you create the [workbookPivotTable](../resources/workbookpivottable.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookpivottable_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/pivotTables
Content-type: application/json
Content-length: 85

{
  "@odata.type": "#microsoft.graph.workbookPivotTable",
  "name": "Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookpivottable"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 134

{
  "@odata.type": "#microsoft.graph.workbookPivotTable",
  "id": "e056142d-142d-e056-2d14-56e02d1456e0",
  "name": "Name value"
}
```

