---
title: "Add tables"
description: "Add tables by posting to the tables collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add tables

Namespace: microsoft.graph

Add tables by posting to the tables collection.

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
POST /me/drive/items/{driveItemId}/workbook/tables/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [workbookTable](../resources/workbooktable.md) object.

The following table shows the properties that are required when you create the [workbookTable](../resources/workbooktable.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|highlightFirstColumn|Boolean||
|highlightLastColumn|Boolean||
|legacyId|String||
|name|String||
|showBandedColumns|Boolean||
|showBandedRows|Boolean||
|showFilterButton|Boolean||
|showHeaders|Boolean||
|showTotals|Boolean||
|style|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookTable](../resources/workbooktable.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbooktable_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/tables
Content-type: application/json
Content-length: 339

{
  "@odata.type": "#microsoft.graph.workbookTable",
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "legacyId": "Legacy Id value",
  "name": "Name value",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "Style value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooktable"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 388

{
  "@odata.type": "#microsoft.graph.workbookTable",
  "id": "da455bba-5bba-da45-ba5b-45daba5b45da",
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "legacyId": "Legacy Id value",
  "name": "Name value",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "Style value"
}
```

