---
title: "educationSchool resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSchool resource type


Namespace: microsoft.graph




Inherits from [educationOrganization](../resources/educationorganization.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSchool](../api/educationschool-get.md)|[educationSchool](../resources/educationschool.md)|Read properties and relationships of the [educationSchool](../resources/educationschool.md) object.|
|[Update educationSchool](../api/educationschool-update.md)|[educationSchool](../resources/educationschool.md)|Update the properties of a [educationSchool](../resources/educationschool.md) object.|
|[List classes](../api/educationschool-list-classes.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the classes navigation property.|
|[Create classes](../api/educationschool-post-classes.md)|[educationClass](../resources/educationclass.md)|Create classes by posting to the classes collection.|
|[List users](../api/educationschool-list-users.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the users navigation property.|
|[Create users](../api/educationschool-post-users.md)|[educationUser](../resources/educationuser.md)|Create users by posting to the users collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)||
|createdBy|[identitySet](../resources/identityset.md)||
|description|String| Inherited from [educationOrganization](../resources/educationorganization.md)|
|displayName|String| Inherited from [educationOrganization](../resources/educationorganization.md)|
|externalId|String||
|externalPrincipalId|String||
|externalSource|Enumeration| Inherited from [educationOrganization](../resources/educationorganization.md). Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|fax|String||
|highestGrade|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lowestGrade|String||
|phone|String||
|principalEmail|String||
|principalName|String||
|schoolNumber|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|classes|[educationClass](../resources/educationclass.md) collection||
|users|[educationUser](../resources/educationuser.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSchool",
  "baseType": "microsoft.graph.educationOrganization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```

