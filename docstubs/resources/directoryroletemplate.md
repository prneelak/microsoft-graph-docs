---
title: "directoryRoleTemplate resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# directoryRoleTemplate resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryRoleTemplates](../api/directoryroletemplate-list.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md) collection|List properties and relationships of the [directoryRoleTemplate](../resources/directoryroletemplate.md) objects.|
|[Get directoryRoleTemplate](../api/directoryroletemplate-get.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md)|Read properties and relationships of the [directoryRoleTemplate](../resources/directoryroletemplate.md) object.|
|[Create directoryRoleTemplate](../api/directoryroletemplate-post-directoryroletemplates.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md)|Create a new [directoryRoleTemplate](../resources/directoryroletemplate.md) object.|
|[Delete directoryRoleTemplate](../api/directoryroletemplate-delete.md)|None|Deletes a [directoryRoleTemplate](../resources/directoryroletemplate.md).|
|[Update directoryRoleTemplate](../api/directoryroletemplate-update.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md)|Update the properties of a [directoryRoleTemplate](../resources/directoryroletemplate.md) object.|
|[checkMemberGroups](../api/directoryroletemplate-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/directoryroletemplate-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/directoryroletemplate-getmembergroups.md)|String collection||
|[getMemberObjects](../api/directoryroletemplate-getmemberobjects.md)|String collection||
|[restore](../api/directoryroletemplate-restore.md)|[directoryObject](../resources/directoryobject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryRoleTemplate",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```

