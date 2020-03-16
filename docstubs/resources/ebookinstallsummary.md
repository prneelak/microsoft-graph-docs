---
title: "eBookInstallSummary resource type"
description: "Contains properties for the installation summary of a book for a device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# eBookInstallSummary resource type


Namespace: microsoft.graph

Contains properties for the installation summary of a book for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get eBookInstallSummary](../api/ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Read properties and relationships of the [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|
|[Update eBookInstallSummary](../api/ebookinstallsummary-update.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Update the properties of a [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|Number of Devices that have failed to install this book.|
|failedUserCount|Int32|Number of Users that have 1 or more device that failed to install this book.|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Number of Devices that have successfully installed this book.|
|installedUserCount|Int32|Number of Users whose devices have all succeeded to install this book.|
|notInstalledDeviceCount|Int32|Number of Devices that does not have this book installed.|
|notInstalledUserCount|Int32|Number of Users that did not install this book.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```

