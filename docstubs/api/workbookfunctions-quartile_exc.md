---
title: "quartile_Exc"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# quartile_Exc

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
POST /me/drive/items/{driveItemId}/workbook/functions/quartile_Exc
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|array|[Json](../resources/json.md)||
|quart|[Json](../resources/json.md)||



## Response
If successful, this action returns a `200 OK` response code and a [workbookFunctionResult](../resources/workbookfunctionresult.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbookfunctions_quartile_exc"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/functions/quartile_Exc

Content-type: application/json
Content-length: 129

{
  "array": {
    "@odata.type": "microsoft.graph.Json"
  },
  "quart": {
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
    "id": "43614f42-4f42-4361-424f-6143424f6143",
    "error": "Error value",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

