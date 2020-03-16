---
title: "permission resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# permission resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get permission](../api/permission-get.md)|[permission](../resources/permission.md)|Read properties and relationships of the [permission](../resources/permission.md) object.|
|[Update permission](../api/permission-update.md)|[permission](../resources/permission.md)|Update the properties of a [permission](../resources/permission.md) object.|
|[List permissions](../api/driveitem-list-permissions.md)|[permission](../resources/permission.md) collection|Get the permissions from the permissions navigation property.|
|[Add permissions](../api/driveitem-post-permissions.md)|[permission](../resources/permission.md)|Add permissions by posting to the permissions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|grantedTo|[identitySet](../resources/identityset.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|inheritedFrom|[itemReference](../resources/itemreference.md)||
|invitation|[sharingInvitation](../resources/sharinginvitation.md)||
|link|[sharingLink](../resources/sharinglink.md)||
|roles|String collection||
|shareId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.permission",
  "id": "String (identifier)",
  "grantedTo": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "inheritedFrom": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "invitation": {
    "@odata.type": "microsoft.graph.sharingInvitation"
  },
  "link": {
    "@odata.type": "microsoft.graph.sharingLink"
  },
  "roles": [
    "String"
  ],
  "shareId": "String"
}
```

