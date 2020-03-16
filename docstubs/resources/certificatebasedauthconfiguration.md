---
title: "certificateBasedAuthConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# certificateBasedAuthConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-get.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Read properties and relationships of the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.|
|[Update certificateBasedAuthConfiguration](../api/certificatebasedauthconfiguration-update.md)|[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)|Update the properties of a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificateAuthorities|[certificateAuthority](../resources/certificateauthority.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
  "id": "String (identifier)",
  "certificateAuthorities": [
    {
      "@odata.type": "microsoft.graph.certificateAuthority"
    }
  ]
}
```

