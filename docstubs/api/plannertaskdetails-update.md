---
title: "Update plannerTaskDetails"
description: "Update the properties of a plannerTaskDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerTaskDetails

Namespace: microsoft.graph

Update the properties of a [plannerTaskDetails](../resources/plannertaskdetails.md) object.

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
PATCH /me/planner/tasks/{plannerTaskId}/details
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerTaskDetails](../resources/plannertaskdetails.md) object.

The following table shows the properties that are required when you create the [plannerTaskDetails](../resources/plannertaskdetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|previewType|Enumeration|. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|references|[plannerExternalReferences](../resources/plannerexternalreferences.md)||
|checklist|[plannerChecklistItems](../resources/plannerchecklistitems.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_plannertaskdetails"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/planner/tasks/{plannerTaskId}/details
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "description": "Description value",
  "previewType": "String",
  "references": {
    "@odata.type": "microsoft.graph.plannerExternalReferences"
  },
  "checklist": {
    "@odata.type": "microsoft.graph.plannerChecklistItems"
  }
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
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "id": "a14778f4-78f4-a147-f478-47a1f47847a1",
  "description": "Description value",
  "previewType": "String",
  "references": {
    "@odata.type": "microsoft.graph.plannerExternalReferences"
  },
  "checklist": {
    "@odata.type": "microsoft.graph.plannerChecklistItems"
  }
}
```

