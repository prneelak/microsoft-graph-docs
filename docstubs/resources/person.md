---
title: "person resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# person resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get person](../api/person-get.md)|[person](../resources/person.md)|Read properties and relationships of the [person](../resources/person.md) object.|
|[Update person](../api/person-update.md)|[person](../resources/person.md)|Update the properties of a [person](../resources/person.md) object.|
|[List people](../api/user-list-people.md)|[person](../resources/person.md) collection|Get the persons from the people navigation property.|
|[Add people](../api/user-post-people.md)|[person](../resources/person.md)|Add people by posting to the people collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|birthday|String||
|companyName|String||
|department|String||
|displayName|String||
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|imAddress|String||
|isFavorite|Boolean||
|jobTitle|String||
|officeLocation|String||
|personNotes|String||
|personType|[personType](../resources/persontype.md)||
|phones|[phone](../resources/phone.md) collection||
|postalAddresses|[location](../resources/location.md) collection||
|profession|String||
|scoredEmailAddresses|[scoredEmailAddress](../resources/scoredemailaddress.md) collection||
|surname|String||
|userPrincipalName|String||
|websites|[website](../resources/website.md) collection||
|yomiCompany|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.person",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.person",
  "id": "String (identifier)",
  "displayName": "String",
  "givenName": "String",
  "surname": "String",
  "birthday": "String",
  "personNotes": "String",
  "isFavorite": true,
  "scoredEmailAddresses": [
    {
      "@odata.type": "microsoft.graph.scoredEmailAddress"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "websites": [
    {
      "@odata.type": "microsoft.graph.website"
    }
  ],
  "jobTitle": "String",
  "companyName": "String",
  "yomiCompany": "String",
  "department": "String",
  "officeLocation": "String",
  "profession": "String",
  "personType": {
    "@odata.type": "microsoft.graph.personType"
  },
  "userPrincipalName": "String",
  "imAddress": "String"
}
```

