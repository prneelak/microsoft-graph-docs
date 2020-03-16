---
title: "identityProvider resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# identityProvider resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List identityProviders](../api/identityprovider-list.md)|[identityProvider](../resources/identityprovider.md) collection|List properties and relationships of the [identityProvider](../resources/identityprovider.md) objects.|
|[Get identityProvider](../api/identityprovider-get.md)|[identityProvider](../resources/identityprovider.md)|Read properties and relationships of the [identityProvider](../resources/identityprovider.md) object.|
|[Create identityProvider](../api/identityprovider-post-identityproviders.md)|[identityProvider](../resources/identityprovider.md)|Create a new [identityProvider](../resources/identityprovider.md) object.|
|[Delete identityProvider](../api/identityprovider-delete.md)|None|Deletes a [identityProvider](../resources/identityprovider.md).|
|[Update identityProvider](../api/identityprovider-update.md)|[identityProvider](../resources/identityprovider.md)|Update the properties of a [identityProvider](../resources/identityprovider.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientId|String||
|clientSecret|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityProvider",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityProvider",
  "id": "String (identifier)",
  "type": "String",
  "name": "String",
  "clientId": "String",
  "clientSecret": "String"
}
```

