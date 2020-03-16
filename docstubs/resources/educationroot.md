---
title: "educationRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationRoot resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationRoot](../api/educationroot-get.md)|[educationRoot](../resources/educationroot.md)|Read properties and relationships of the [educationRoot](../resources/educationroot.md) object.|
|[Update educationRoot](../api/educationroot-update.md)|[educationRoot](../resources/educationroot.md)|Update the properties of a [educationRoot](../resources/educationroot.md) object.|
|[List classes](../api/educationroot-list-classes.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the classes navigation property.|
|[Add classes](../api/educationroot-post-classes.md)|[educationClass](../resources/educationclass.md)|Add classes by posting to the classes collection.|
|[List schools](../api/educationroot-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchools from the schools navigation property.|
|[Add schools](../api/educationroot-post-schools.md)|[educationSchool](../resources/educationschool.md)|Add schools by posting to the schools collection.|
|[List users](../api/educationroot-list-users.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the users navigation property.|
|[Add users](../api/educationroot-post-users.md)|[educationUser](../resources/educationuser.md)|Add users by posting to the users collection.|
|[Get educationUser](../api/educationuser-get.md)|[educationUser](../resources/educationuser.md)|Read properties and relationships of the [educationUser](../resources/educationuser.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|classes|[educationClass](../resources/educationclass.md) collection||
|me|[educationUser](../resources/educationuser.md)||
|schools|[educationSchool](../resources/educationschool.md) collection||
|users|[educationUser](../resources/educationuser.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationRoot",
  "id": "String (identifier)"
}
```

