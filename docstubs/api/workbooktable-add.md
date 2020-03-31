---
title: "add"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# add

Namespace: microsoft.graph



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
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/tables/add
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/add
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|address|String||
|hasHeaders|Boolean||



## Response
If successful, this action returns a `200 OK` response code and a [workbookTable](../resources/workbooktable.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbooktable_add"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/tables/add

Content-type: application/json
Content-length: 57

{
  "address": "Address value",
  "hasHeaders": true
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 431

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookTable",
    "id": "6024e159-e159-6024-59e1-246059e12460",
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
}
```

