---
title: "plannerTask resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerTask resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerTask](../api/plannertask-get.md)|[plannerTask](../resources/plannertask.md)|Read properties and relationships of the [plannerTask](../resources/plannertask.md) object.|
|[Update plannerTask](../api/plannertask-update.md)|[plannerTask](../resources/plannertask.md)|Update the properties of a [plannerTask](../resources/plannertask.md) object.|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Read properties and relationships of the [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Read properties and relationships of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Get plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)|Read properties and relationships of the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|Read properties and relationships of the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeChecklistItemCount|Int32||
|appliedCategories|[plannerAppliedCategories](../resources/plannerappliedcategories.md)||
|assigneePriority|String||
|assignments|[plannerAssignments](../resources/plannerassignments.md)||
|bucketId|String||
|checklistItemCount|Int32||
|completedBy|[identitySet](../resources/identityset.md)||
|completedDateTime|DateTimeOffset||
|conversationThreadId|String||
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset||
|dueDateTime|DateTimeOffset||
|hasDescription|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHint|String||
|percentComplete|Int32||
|planId|String||
|previewType|Enumeration|. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|referenceCount|Int32||
|startDateTime|DateTimeOffset||
|title|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)||
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)||
|details|[plannerTaskDetails](../resources/plannertaskdetails.md)||
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTask",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "planId": "String",
  "bucketId": "String",
  "title": "String",
  "orderHint": "String",
  "assigneePriority": "String",
  "percentComplete": 1024,
  "startDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "previewType": "String",
  "completedDateTime": "String (timestamp)",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "referenceCount": 1024,
  "checklistItemCount": 1024,
  "activeChecklistItemCount": 1024,
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "conversationThreadId": "String"
}
```

