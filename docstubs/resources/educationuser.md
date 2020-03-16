---
title: "educationUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationUser resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationUser](../api/educationuser-get.md)|[educationUser](../resources/educationuser.md)|Read properties and relationships of the [educationUser](../resources/educationuser.md) object.|
|[Update educationUser](../api/educationuser-update.md)|[educationUser](../resources/educationuser.md)|Update the properties of a [educationUser](../resources/educationuser.md) object.|
|[List schools](../api/educationuser-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchools from the schools navigation property.|
|[Create schools](../api/educationuser-post-schools.md)|[educationSchool](../resources/educationschool.md)|Create schools by posting to the schools collection.|
|[List classes](../api/educationuser-list-classes.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the classes navigation property.|
|[Create classes](../api/educationuser-post-classes.md)|[educationClass](../resources/educationclass.md)|Create classes by posting to the classes collection.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean||
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection||
|businessPhones|String collection||
|createdBy|[identitySet](../resources/identityset.md)||
|department|String||
|displayName|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|mail|String||
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)||
|mailNickname|String||
|middleName|String||
|mobilePhone|String||
|officeLocation|String||
|passwordPolicies|String||
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)||
|preferredLanguage|String||
|primaryRole|Enumeration|. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`.|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection||
|refreshTokensValidFromDateTime|DateTimeOffset||
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)||
|showInAddressList|Boolean||
|student|[educationStudent](../resources/educationstudent.md)||
|surname|String||
|teacher|[educationTeacher](../resources/educationteacher.md)||
|usageLocation|String||
|userPrincipalName|String||
|userType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|classes|[educationClass](../resources/educationclass.md) collection||
|schools|[educationSchool](../resources/educationschool.md) collection||
|user|[user](../resources/user.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "String (identifier)",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": true,
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

