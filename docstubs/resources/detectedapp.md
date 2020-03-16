---
title: "detectedApp resource type"
description: "A managed or unmanaged app that is installed on a managed device. Unmanaged apps will only appear for devices marked as corporate owned."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# detectedApp resource type


Namespace: microsoft.graph

A managed or unmanaged app that is installed on a managed device. Unmanaged apps will only appear for devices marked as corporate owned.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get detectedApp](../api/detectedapp-get.md)|[detectedApp](../resources/detectedapp.md)|Read properties and relationships of the [detectedApp](../resources/detectedapp.md) object.|
|[Update detectedApp](../api/detectedapp-update.md)|[detectedApp](../resources/detectedapp.md)|Update the properties of a [detectedApp](../resources/detectedapp.md) object.|
|[List managedDevices](../api/detectedapp-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Create managedDevices](../api/detectedapp-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Create managedDevices by posting to the managedDevices collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int32|The number of devices that have installed this application|
|displayName|String|Name of the discovered application. Read-only|
|id|String| Inherited from [entity](../resources/entity.md)|
|sizeInByte|Int64|Discovered application size in bytes. Read-only|
|version|String|Version of the discovered application. Read-only|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/manageddevice.md) collection|The devices that have the discovered application installed|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```

