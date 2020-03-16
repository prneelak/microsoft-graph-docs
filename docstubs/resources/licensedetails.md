---
title: "licenseDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# licenseDetails resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get licenseDetails](../api/licensedetails-get.md)|[licenseDetails](../resources/licensedetails.md)|Read properties and relationships of the [licenseDetails](../resources/licensedetails.md) object.|
|[Update licenseDetails](../api/licensedetails-update.md)|[licenseDetails](../resources/licensedetails.md)|Update the properties of a [licenseDetails](../resources/licensedetails.md) object.|
|[List licenseDetails](../api/user-list-licensedetails.md)|[licenseDetails](../resources/licensedetails.md) collection|Get the licenseDetailses from the licenseDetails navigation property.|
|[Add licenseDetails](../api/user-post-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Add licenseDetails by posting to the licenseDetails collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|servicePlans|[servicePlanInfo](../resources/serviceplaninfo.md) collection||
|skuId|Guid||
|skuPartNumber|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "id": "String (identifier)",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
}
```

