---
title: "permut"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# permut

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
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/functions/permut
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
|number|[Json](../resources/json.md)||
|numberChosen|[Json](../resources/json.md)||



## Response
If successful, this action returns a `200 OK` response code and a [workbookFunctionResult](../resources/workbookfunctionresult.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbookfunctions_permut"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/functions/permut

Content-type: application/json
Content-length: 137

{
  "number": {
    "@odata.type": "microsoft.graph.Json"
  },
  "numberChosen": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookfunctionresult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "id": "19de6bef-6bef-19de-ef6b-de19ef6bde19",
    "error": "Error value",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

