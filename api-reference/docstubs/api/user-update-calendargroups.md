---
title: "Update calendarGroups"
description: "Update the properties of a calendarGroups object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update calendarGroups

Namespace: microsoft.graph

Update the properties of a calendarGroups object.

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
PATCH /me/calendarGroups
PATCH /users/{usersId}/calendarGroups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [calendarGroup](../resources/calendargroup.md) object.

The following table shows the properties that are required when you create the [calendarGroup](../resources/calendargroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|classId|Guid|**TODO: Add Description**|
|changeKey|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [calendarGroup](../resources/calendargroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_calendargroups"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/calendarGroups
Content-Type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "name": "String",
  "classId": "Guid",
  "changeKey": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "id": "c61e722d-722d-c61e-2d72-1ec62d721ec6",
  "name": "String",
  "classId": "Guid",
  "changeKey": "String"
}
```

