---
title: "managedMobileApp resource type"
description: "The identifier for the deployment an app."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedMobileApp resource type


Namespace: microsoft.graph

The identifier for the deployment an app.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedMobileApp](../api/managedmobileapp-get.md)|[managedMobileApp](../resources/managedmobileapp.md)|Read properties and relationships of the [managedMobileApp](../resources/managedmobileapp.md) object.|
|[Update managedMobileApp](../api/managedmobileapp-update.md)|[managedMobileApp](../resources/managedmobileapp.md)|Update the properties of a [managedMobileApp](../resources/managedmobileapp.md) object.|
|[List apps](../api/androidmanagedappprotection-list-apps.md)|[managedMobileApp](../resources/managedmobileapp.md) collection|Get the managedMobileApps from the apps navigation property.|
|[Add apps](../api/androidmanagedappprotection-post-apps.md)|[managedMobileApp](../resources/managedmobileapp.md)|Add apps by posting to the apps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The identifier for an app with it's operating system type.|
|version|String|Version of the entity.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "id": "String (identifier)",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "String"
}
```

