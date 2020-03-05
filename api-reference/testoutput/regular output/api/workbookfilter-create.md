---
title: "Create workbookFilter"
description: "Create a new workbookFilter object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookFilter

Namespace: microsoft.graph

Create a new [workbookFilter](../resources/workbookfilter.md) object.

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
POST ** Collection URI for microsoft.graph.workbookFilter not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookFilter](../resources/workbookfilter.md) object.

The following table shows the properties that are required when you create the [workbookFilter](../resources/workbookfilter.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|criteria|[workbookFilterCriteria](../resources/workbookfiltercriteria.md)||



## Response
If successful, this method returns a `201 Created` response code and a [workbookFilter](../resources/workbookfilter.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookfilter_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookFilter not found
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria",
    "color": "Color value",
    "criterion1": "Criterion1 value",
    "criterion2": "Criterion2 value",
    "dynamicCriteria": "Dynamic Criteria value",
    "filterOn": "Filter On value",
    "icon": {
      "@odata.type": "microsoft.graph.workbookIcon",
      "index": 5,
      "set": "Set value"
    },
    "operator": "Operator value",
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookfilter"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 609

{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "id": "b113c2ce-c2ce-b113-cec2-13b1cec213b1",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria",
    "color": "Color value",
    "criterion1": "Criterion1 value",
    "criterion2": "Criterion2 value",
    "dynamicCriteria": "Dynamic Criteria value",
    "filterOn": "Filter On value",
    "icon": {
      "@odata.type": "microsoft.graph.workbookIcon",
      "index": 5,
      "set": "Set value"
    },
    "operator": "Operator value",
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

