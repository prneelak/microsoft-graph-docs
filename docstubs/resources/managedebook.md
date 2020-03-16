---
title: "managedEBook resource type"
description: "An abstract class containing the base properties for Managed eBook."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedEBook resource type


Namespace: microsoft.graph

An abstract class containing the base properties for Managed eBook.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedEBook](../api/managedebook-get.md)|[managedEBook](../resources/managedebook.md)|Read properties and relationships of the [managedEBook](../resources/managedebook.md) object.|
|[assign](../api/managedebook-assign.md)|None||
|[List assignments](../api/managedebook-list-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md) collection|Get the managedEBookAssignments from the assignments navigation property.|
|[Add assignments](../api/managedebook-post-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Add assignments by posting to the assignments collection.|
|[Get eBookInstallSummary](../api/ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Read properties and relationships of the [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|
|[List deviceStates](../api/managedebook-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Add deviceStates](../api/managedebook-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Add deviceStates by posting to the deviceStates collection.|
|[List userStateSummary](../api/managedebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Add userStateSummary](../api/managedebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Add userStateSummary by posting to the userStateSummary collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time when the eBook file was created.|
|description|String|Description.|
|displayName|String|Name of the eBook.|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url.|
|largeCover|[mimeContent](../resources/mimecontent.md)|Book cover.|
|lastModifiedDateTime|DateTimeOffset|The date and time when the eBook was last modified.|
|privacyInformationUrl|String|The privacy statement Url.|
|publishedDateTime|DateTimeOffset|The date and time when the eBook was published.|
|publisher|String|Publisher.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/managedebookassignment.md) collection|The list of assignments for this eBook.|
|deviceStates|[deviceInstallState](../resources/deviceinstallstate.md) collection|The list of installation states for this eBook.|
|installSummary|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Mobile App Install Summary.|
|userStateSummary|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|The list of installation states for this eBook.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```

