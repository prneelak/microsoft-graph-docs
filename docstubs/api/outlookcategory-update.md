---
title: "Update outlookCategory"
description: "Update the properties of a outlookCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update outlookCategory

Namespace: microsoft.graph

Update the properties of a [outlookCategory](../resources/outlookcategory.md) object.

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
PATCH /me/outlook/masterCategories/{outlookCategoryId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [outlookCategory](../resources/outlookcategory.md) object.

The following table shows the properties that are required when you create the [outlookCategory](../resources/outlookcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|color|Enumeration|. Possible values are: `preset0`, `preset1`, `preset2`, `preset3`, `preset4`, `preset5`, `preset6`, `preset7`, `preset8`, `preset9`, `preset10`, `preset11`, `preset12`, `preset13`, `preset14`, `preset15`, `preset16`, `preset17`, `preset18`, `preset19`, `preset20`, `preset21`, `preset22`, `preset23`, `preset24`, `none`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [outlookCategory](../resources/outlookcategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/outlook/masterCategories/{outlookCategoryId}
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "displayName": "Display Name value",
  "color": "String"
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
Content-Length: 168

{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "id": "683dd2c3-d2c3-683d-c3d2-3d68c3d23d68",
  "displayName": "Display Name value",
  "color": "String"
}
```

