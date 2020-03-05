---
title: "Create workbookWorksheet"
description: "Create a new workbookWorksheet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookWorksheet

Namespace: microsoft.graph

Create a new [workbookWorksheet](../resources/workbookworksheet.md) object.

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
POST /me/drive/items/{driveItemId}/workbook/worksheets
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookWorksheet](../resources/workbookworksheet.md) object.

The following table shows the properties that are required when you create the [workbookWorksheet](../resources/workbookworksheet.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|position|Int32||
|visibility|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookworksheet_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/worksheets
Content-type: application/json
Content-length: 139

{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "name": "Name value",
  "position": 8,
  "visibility": "Visibility value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookworksheet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 188

{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "id": "df2a93d4-93d4-df2a-d493-2adfd4932adf",
  "name": "Name value",
  "position": 8,
  "visibility": "Visibility value"
}
```

