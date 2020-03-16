---
title: "Update workbookWorksheetProtection"
description: "Update the properties of a workbookWorksheetProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookWorksheetProtection

Namespace: microsoft.graph

Update the properties of a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/protection
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.

The following table shows the properties that are required when you create the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|options|[workbookWorksheetProtectionOptions](../resources/workbookworksheetprotectionoptions.md)||
|protected|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookworksheetprotection"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/protection
Content-type: application/json
Content-length: 527

{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "options": {
    "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions",
    "allowAutoFilter": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertHyperlinks": true,
    "allowInsertRows": true,
    "allowPivotTables": true,
    "allowSort": true
  },
  "protected": true
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
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "id": "8c6bb640-b640-8c6b-40b6-6b8c40b66b8c",
  "options": {
    "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions",
    "allowAutoFilter": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertHyperlinks": true,
    "allowInsertRows": true,
    "allowPivotTables": true,
    "allowSort": true
  },
  "protected": true
}
```

