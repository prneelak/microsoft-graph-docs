---
title: "Update charts"
description: "Update the properties of a charts object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update charts

Namespace: microsoft.graph

Update the properties of a charts object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [workbookChart](../resources/workbookchart.md) object.

The following table shows the properties that are required when you create the [workbookChart](../resources/workbookchart.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|height|Double|**TODO: Add Description**|
|left|Double|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|top|Double|**TODO: Add Description**|
|width|Double|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChart](../resources/workbookchart.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_charts"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.workbookChart",
  "height": "Double",
  "left": "Double",
  "name": "Name value",
  "top": "Double",
  "width": "Double"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookChart",
  "id": "01a4f498-f498-01a4-98f4-a40198f4a401",
  "height": "Double",
  "left": "Double",
  "name": "Name value",
  "top": "Double",
  "width": "Double"
}
```

