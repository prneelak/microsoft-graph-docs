---
title: "educationClass resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationClass resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationClass](../api/educationclass-get.md)|[educationClass](../resources/educationclass.md)|Read properties and relationships of the [educationClass](../resources/educationclass.md) object.|
|[Update educationClass](../api/educationclass-update.md)|[educationClass](../resources/educationclass.md)|Update the properties of a [educationClass](../resources/educationclass.md) object.|
|[List schools](../api/educationclass-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchools from the schools navigation property.|
|[Create schools](../api/educationclass-post-schools.md)|[educationSchool](../resources/educationschool.md)|Create schools by posting to the schools collection.|
|[List members](../api/educationclass-list-members.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the members navigation property.|
|[Create members](../api/educationclass-post-members.md)|[educationUser](../resources/educationuser.md)|Create members by posting to the members collection.|
|[List teachers](../api/educationclass-list-teachers.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the teachers navigation property.|
|[Create teachers](../api/educationclass-post-teachers.md)|[educationUser](../resources/educationuser.md)|Create teachers by posting to the teachers collection.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read properties and relationships of the [group](../resources/group.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classCode|String||
|createdBy|[identitySet](../resources/identityset.md)||
|description|String||
|displayName|String||
|externalId|String||
|externalName|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|mailNickname|String||
|term|[educationTerm](../resources/educationterm.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|group|[group](../resources/group.md)||
|members|[educationUser](../resources/educationuser.md) collection||
|schools|[educationSchool](../resources/educationschool.md) collection||
|teachers|[educationUser](../resources/educationuser.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationClass",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "String (identifier)",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm",
    "startDate": "Date",
    "endDate": "Date"
  }
}
```

