---
title: "extensionProperty resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# extensionProperty resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get extensionProperty](../api/extensionproperty-get.md)|[extensionProperty](../resources/extensionproperty.md)|Read properties and relationships of the [extensionProperty](../resources/extensionproperty.md) object.|
|[Update extensionProperty](../api/extensionproperty-update.md)|[extensionProperty](../resources/extensionproperty.md)|Update the properties of a [extensionProperty](../resources/extensionproperty.md) object.|
|[checkMemberGroups](../api/extensionproperty-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/extensionproperty-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/extensionproperty-getmembergroups.md)|String collection||
|[getMemberObjects](../api/extensionproperty-getmemberobjects.md)|String collection||
|[restore](../api/extensionproperty-restore.md)|[directoryObject](../resources/directoryobject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String||
|dataType|String||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isSyncedFromOnPremises|Boolean||
|name|String||
|targetObjects|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "name": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "targetObjects": [
    "String"
  ]
}
```

