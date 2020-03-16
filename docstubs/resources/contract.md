---
title: "contract resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# contract resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List contracts](../api/contract-list.md)|[contract](../resources/contract.md) collection|List properties and relationships of the [contract](../resources/contract.md) objects.|
|[Get contract](../api/contract-get.md)|[contract](../resources/contract.md)|Read properties and relationships of the [contract](../resources/contract.md) object.|
|[Create contract](../api/contract-post-contracts.md)|[contract](../resources/contract.md)|Create a new [contract](../resources/contract.md) object.|
|[Delete contract](../api/contract-delete.md)|None|Deletes a [contract](../resources/contract.md).|
|[Update contract](../api/contract-update.md)|[contract](../resources/contract.md)|Update the properties of a [contract](../resources/contract.md) object.|
|[checkMemberGroups](../api/contract-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/contract-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/contract-getmembergroups.md)|String collection||
|[getMemberObjects](../api/contract-getmemberobjects.md)|String collection||
|[restore](../api/contract-restore.md)|[directoryObject](../resources/directoryobject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contractType|String||
|customerId|Guid||
|defaultDomainName|String||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contract",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contract",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String"
}
```

