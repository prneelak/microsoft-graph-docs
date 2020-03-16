---
title: "directoryRole resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# directoryRole resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryRoles](../api/directoryrole-list.md)|[directoryRole](../resources/directoryrole.md) collection|List properties and relationships of the [directoryRole](../resources/directoryrole.md) objects.|
|[Get directoryRole](../api/directoryrole-get.md)|[directoryRole](../resources/directoryrole.md)|Read properties and relationships of the [directoryRole](../resources/directoryrole.md) object.|
|[Create directoryRole](../api/directoryrole-post-directoryroles.md)|[directoryRole](../resources/directoryrole.md)|Create a new [directoryRole](../resources/directoryrole.md) object.|
|[Delete directoryRole](../api/directoryrole-delete.md)|None|Deletes a [directoryRole](../resources/directoryrole.md).|
|[Update directoryRole](../api/directoryrole-update.md)|[directoryRole](../resources/directoryrole.md)|Update the properties of a [directoryRole](../resources/directoryrole.md) object.|
|[delta](../api/directoryrole-delta.md)|[directoryRole](../resources/directoryrole.md) collection||
|[checkMemberGroups](../api/directoryrole-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/directoryrole-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/directoryrole-getmembergroups.md)|String collection||
|[getMemberObjects](../api/directoryrole-getmemberobjects.md)|String collection||
|[restore](../api/directoryrole-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[List members](../api/directoryrole-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Create members](../api/directoryrole-post-members.md)|[directoryObject](../resources/directoryobject.md)|Create members by posting to the members collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|roleTemplateId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|members|[directoryObject](../resources/directoryobject.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryRole",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "roleTemplateId": "String"
}
```

