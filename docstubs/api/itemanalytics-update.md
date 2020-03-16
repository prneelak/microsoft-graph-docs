---
title: "Update itemAnalytics"
description: "Update the properties of a itemAnalytics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update itemAnalytics

Namespace: microsoft.graph

Update the properties of a [itemAnalytics](../resources/itemanalytics.md) object.

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
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [itemAnalytics](../resources/itemanalytics.md) object.

The following table shows the properties that are required when you create the [itemAnalytics](../resources/itemanalytics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [itemAnalytics](../resources/itemanalytics.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_itemanalytics"
}
-->
``` http

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
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.itemAnalytics",
  "id": "55383e51-3e51-5538-513e-3855513e3855"
}
```

