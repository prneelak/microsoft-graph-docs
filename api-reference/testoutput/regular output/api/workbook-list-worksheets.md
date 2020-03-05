---
title: "List worksheets"
description: "Get the workbookWorksheets from the worksheets navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List worksheets

Namespace: microsoft.graph

Get the workbookWorksheets from the worksheets navigation property.

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
GET /me/drive/items/{driveItemId}/workbook/worksheets
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookWorksheet](../resources/workbookworksheet.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheet"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/worksheets
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookworksheet)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookWorksheet",
      "id": "df2a93d4-93d4-df2a-d493-2adfd4932adf",
      "name": "Name value",
      "position": 8,
      "visibility": "Visibility value"
    }
  ]
}
```

