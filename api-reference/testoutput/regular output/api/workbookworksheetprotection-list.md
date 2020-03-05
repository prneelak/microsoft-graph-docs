---
title: "List workbookWorksheetProtections"
description: "List properties and relationships of the workbookWorksheetProtection objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookWorksheetProtections

Namespace: microsoft.graph

List properties and relationships of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookWorksheetProtection not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheetprotection"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookWorksheetProtection not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookworksheetprotection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 677

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
      "id": "2694d3f1-d3f1-2694-f1d3-9426f1d39426",
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
  ]
}
```

