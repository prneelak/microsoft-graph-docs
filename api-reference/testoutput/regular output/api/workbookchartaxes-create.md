---
title: "Create workbookChartAxes"
description: "Create a new workbookChartAxes object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookChartAxes

Namespace: microsoft.graph

Create a new [workbookChartAxes](../resources/workbookchartaxes.md) object.

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
POST ** Collection URI for microsoft.graph.workbookChartAxes not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookChartAxes](../resources/workbookchartaxes.md) object.

The following table shows the properties that are required when you create the [workbookChartAxes](../resources/workbookchartaxes.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [workbookChartAxes](../resources/workbookchartaxes.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookchartaxes_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartAxes not found
Content-type: application/json
Content-length: 59

{
  "@odata.type": "#microsoft.graph.workbookChartAxes"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartaxes"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 108

{
  "@odata.type": "#microsoft.graph.workbookChartAxes",
  "id": "ce29ad75-ad75-ce29-75ad-29ce75ad29ce"
}
```

