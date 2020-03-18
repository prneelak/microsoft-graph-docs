---
title: "oddFPrice"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# oddFPrice

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
POST /me/drive/items/{driveItemId}/workbook/functions/oddFPrice
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
|settlement|[Json](../resources/json.md)||
|maturity|[Json](../resources/json.md)||
|issue|[Json](../resources/json.md)||
|firstCoupon|[Json](../resources/json.md)||
|rate|[Json](../resources/json.md)||
|yld|[Json](../resources/json.md)||
|redemption|[Json](../resources/json.md)||
|frequency|[Json](../resources/json.md)||
|basis|[Json](../resources/json.md)||



## Response
If successful, this action returns a `200 OK` response code and a [workbookFunctionResult](../resources/workbookfunctionresult.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbookfunctions_oddfprice"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/functions/oddFPrice

Content-type: application/json
Content-length: 590

{
  "settlement": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maturity": {
    "@odata.type": "microsoft.graph.Json"
  },
  "issue": {
    "@odata.type": "microsoft.graph.Json"
  },
  "firstCoupon": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rate": {
    "@odata.type": "microsoft.graph.Json"
  },
  "yld": {
    "@odata.type": "microsoft.graph.Json"
  },
  "redemption": {
    "@odata.type": "microsoft.graph.Json"
  },
  "frequency": {
    "@odata.type": "microsoft.graph.Json"
  },
  "basis": {
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
    "id": "1ea471f6-71f6-1ea4-f671-a41ef671a41e",
    "error": "Error value",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

