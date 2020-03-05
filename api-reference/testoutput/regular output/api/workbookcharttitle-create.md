---
title: "Create workbookChartTitle"
description: "Create a new workbookChartTitle object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookChartTitle

Namespace: microsoft.graph

Create a new [workbookChartTitle](../resources/workbookcharttitle.md) object.

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
POST ** Collection URI for microsoft.graph.workbookChartTitle not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookChartTitle](../resources/workbookcharttitle.md) object.

The following table shows the properties that are required when you create the [workbookChartTitle](../resources/workbookcharttitle.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|overlay|Boolean||
|text|String||
|visible|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookcharttitle_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartTitle not found
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "overlay": true,
  "text": "Text value",
  "visible": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookcharttitle"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 174

{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "id": "a493ed52-ed52-a493-52ed-93a452ed93a4",
  "overlay": true,
  "text": "Text value",
  "visible": true
}
```

