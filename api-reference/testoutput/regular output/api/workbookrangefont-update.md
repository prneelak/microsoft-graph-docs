---
title: "Update workbookRangeFont"
description: "Update the properties of a workbookRangeFont object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookRangeFont

Namespace: microsoft.graph

Update the properties of a [workbookRangeFont](../resources/workbookrangefont.md) object.

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
PATCH ** Entity URI for microsoft.graph.workbookRangeFont not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookRangeFont](../resources/workbookrangefont.md) object.

The following table shows the properties that are required when you create the [workbookRangeFont](../resources/workbookrangefont.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|bold|Boolean||
|color|String||
|italic|Boolean||
|name|String||
|size|Double||
|underline|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookRangeFont](../resources/workbookrangefont.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookrangefont"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.workbookRangeFont not found
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.workbookRangeFont",
  "bold": true,
  "color": "Color value",
  "italic": true,
  "name": "Name value",
  "size": "Double",
  "underline": "Underline value"
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
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.workbookRangeFont",
  "id": "3de50d28-0d28-3de5-280d-e53d280de53d",
  "bold": true,
  "color": "Color value",
  "italic": true,
  "name": "Name value",
  "size": "Double",
  "underline": "Underline value"
}
```

