---
title: "managedAppPolicy resource type"
description: "The ManagedAppPolicy resource represents a base type for platform specific policies."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppPolicy resource type


Namespace: microsoft.graph

The ManagedAppPolicy resource represents a base type for platform specific policies.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAppPolicy](../api/managedapppolicy-get.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Read properties and relationships of the [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[targetApps](../api/managedapppolicy-targetapps.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the policy was created.|
|description|String|The policy's description.|
|displayName|String|Policy display name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified.|
|version|String|Version of the entity.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "String"
}
```

