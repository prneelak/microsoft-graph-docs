---
title: "mobileApp resource type"
description: "An abstract class containing the base properties for Intune mobile apps."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileApp resource type


Namespace: microsoft.graph

An abstract class containing the base properties for Intune mobile apps.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileApp](../api/mobileapp-get.md)|[mobileApp](../resources/mobileapp.md)|Read properties and relationships of the [mobileApp](../resources/mobileapp.md) object.|
|[assign](../api/mobileapp-assign.md)|None||
|[List categories](../api/mobileapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategories from the categories navigation property.|
|[Create categories](../api/mobileapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/mobileapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignments from the assignments navigation property.|
|[Add assignments](../api/mobileapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the app was created.|
|description|String|The description of the app.|
|developer|String|The developer of the app.|
|displayName|String|The admin provided or imported title of the app.|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url.|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin.|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon.|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified.|
|notes|String|Notes for the app.|
|owner|String|The owner of the app.|
|privacyInformationUrl|String|The privacy statement Url.|
|publisher|String|The publisher of the app.|
|publishingState|Enumeration|The publishing state for the app. The app cannot be assigned unless the app is published. Possible values are: `notPublished`, `processing`, `published`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app.|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```

