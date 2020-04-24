---
title: "deviceCategory resource type"
description: "Device categories provides a way to organize your devices. Using device categories, company administrators can define their own categories that make sense to their company. These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment. You can filter reports and create dynamic Azure Active Directory device groups based on device categories."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceCategory resource type


Namespace: microsoft.graph

Device categories provides a way to organize your devices. Using device categories, company administrators can define their own categories that make sense to their company. These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment. You can filter reports and create dynamic Azure Active Directory device groups based on device categories.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read the properties and relationships of a [deviceCategory](../resources/devicecategory.md) object.|
|[Update deviceCategory](../api/devicecategory-update.md)|[deviceCategory](../resources/devicecategory.md)|Update the properties of a [deviceCategory](../resources/devicecategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Optional description for the device category.|
|displayName|String|Display name for the device category.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|roleScopeTagIds|String collection|Optional role scope tags for the device category.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

