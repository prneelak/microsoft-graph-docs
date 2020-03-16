---
title: "Update plannerTask"
description: "Update the properties of a plannerTask object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerTask

Namespace: microsoft.graph

Update the properties of a [plannerTask](../resources/plannertask.md) object.

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
PATCH /planner/tasks/{plannerTaskId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerTask](../resources/plannertask.md) object.

The following table shows the properties that are required when you create the [plannerTask](../resources/plannertask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)||
|planId|String||
|bucketId|String||
|title|String||
|orderHint|String||
|assigneePriority|String||
|percentComplete|Int32||
|startDateTime|DateTimeOffset||
|createdDateTime|DateTimeOffset||
|dueDateTime|DateTimeOffset||
|hasDescription|Boolean||
|previewType|Enumeration|. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|completedDateTime|DateTimeOffset||
|completedBy|[identitySet](../resources/identityset.md)||
|referenceCount|Int32||
|checklistItemCount|Int32||
|activeChecklistItemCount|Int32||
|appliedCategories|[plannerAppliedCategories](../resources/plannerappliedcategories.md)||
|assignments|[plannerAssignments](../resources/plannerassignments.md)||
|conversationThreadId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerTask](../resources/plannertask.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/planner/tasks/{plannerTaskId}
Content-type: application/json
Content-length: 1252

{
  "@odata.type": "#microsoft.graph.plannerTask",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "planId": "Plan Id value",
  "bucketId": "Bucket Id value",
  "title": "Title value",
  "orderHint": "Order Hint value",
  "assigneePriority": "Assignee Priority value",
  "percentComplete": 15,
  "startDateTime": "2017-01-01T00:02:40.1232988+03:00",
  "dueDateTime": "2016-12-31T23:58:46.1856943+03:00",
  "hasDescription": true,
  "previewType": "String",
  "completedDateTime": "2017-01-01T00:01:15.9862985+03:00",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "referenceCount": 14,
  "checklistItemCount": 2,
  "activeChecklistItemCount": 8,
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "conversationThreadId": "Conversation Thread Id value"
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
Content-Length: 1360

{
  "@odata.type": "#microsoft.graph.plannerTask",
  "id": "a7448b63-8b63-a744-638b-44a7638b44a7",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "planId": "Plan Id value",
  "bucketId": "Bucket Id value",
  "title": "Title value",
  "orderHint": "Order Hint value",
  "assigneePriority": "Assignee Priority value",
  "percentComplete": 15,
  "startDateTime": "2017-01-01T00:02:40.1232988+03:00",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "dueDateTime": "2016-12-31T23:58:46.1856943+03:00",
  "hasDescription": true,
  "previewType": "String",
  "completedDateTime": "2017-01-01T00:01:15.9862985+03:00",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "referenceCount": 14,
  "checklistItemCount": 2,
  "activeChecklistItemCount": 8,
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "conversationThreadId": "Conversation Thread Id value"
}
```

