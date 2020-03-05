---
title: "List workbookChartLineFormats"
description: "List properties and relationships of the workbookChartLineFormat objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookChartLineFormats

Namespace: microsoft.graph

List properties and relationships of the [workbookChartLineFormat](../resources/workbookchartlineformat.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookChartLineFormat not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookChartLineFormat](../resources/workbookchartlineformat.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookchartlineformat"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookChartLineFormat not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookchartlineformat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookChartLineFormat",
      "id": "c2b88c2c-8c2c-c2b8-2c8c-b8c22c8cb8c2",
      "color": "Color value"
    }
  ]
}
```

