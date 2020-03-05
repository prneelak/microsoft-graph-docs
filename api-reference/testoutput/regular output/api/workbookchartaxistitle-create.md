---
title: "Create workbookChartAxisTitle"
description: "Create a new workbookChartAxisTitle object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookChartAxisTitle

Namespace: microsoft.graph

Create a new [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.

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
POST ** Collection URI for microsoft.graph.workbookChartAxisTitle not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.

The following table shows the properties that are required when you create the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|text|String||
|visible|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartaxistitle_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartAxisTitle not found
Content-type: application/json
Content-length: 109

{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitle",
  "text": "Text value",
  "visible": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartaxistitle"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 158

{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitle",
  "id": "3b8ad2bc-d2bc-3b8a-bcd2-8a3bbcd28a3b",
  "text": "Text value",
  "visible": true
}
```

