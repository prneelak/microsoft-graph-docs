---
title: "Update workbookFilter"
description: "Update the properties of a workbookFilter object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookFilter

Namespace: microsoft.graph

Update the properties of a [workbookFilter](../resources/workbookfilter.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [workbookFilter](../resources/workbookfilter.md) object.

The following table shows the properties that are required when you create the [workbookFilter](../resources/workbookfilter.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|criteria|[workbookFilterCriteria](../resources/workbookfiltercriteria.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookFilter](../resources/workbookfilter.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookfilter"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns/{workbookTableColumnId}/filter
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria",
    "color": "Color value",
    "criterion1": "Criterion1 value",
    "criterion2": "Criterion2 value",
    "dynamicCriteria": "Dynamic Criteria value",
    "filterOn": "Filter On value",
    "icon": {
      "@odata.type": "microsoft.graph.workbookIcon",
      "index": 5,
      "set": "Set value"
    },
    "operator": "Operator value",
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
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
Content-Length: 609

{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "id": "08bb7bca-7bca-08bb-ca7b-bb08ca7bbb08",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria",
    "color": "Color value",
    "criterion1": "Criterion1 value",
    "criterion2": "Criterion2 value",
    "dynamicCriteria": "Dynamic Criteria value",
    "filterOn": "Filter On value",
    "icon": {
      "@odata.type": "microsoft.graph.workbookIcon",
      "index": 5,
      "set": "Set value"
    },
    "operator": "Operator value",
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

