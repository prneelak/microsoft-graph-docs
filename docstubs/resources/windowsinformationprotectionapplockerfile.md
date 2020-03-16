---
title: "windowsInformationProtectionAppLockerFile resource type"
description: "Windows Information Protection AppLocker File"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionAppLockerFile resource type


Namespace: microsoft.graph

Windows Information Protection AppLocker File


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionAppLockerFile](../api/windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|
|[Update windowsInformationProtectionAppLockerFile](../api/windowsinformationprotectionapplockerfile-update.md)|[windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md)|Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/windowsinformationprotectionapplockerfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The friendly name|
|file|Binary|File as a byte array|
|fileHash|String|SHA256 hash of the file|
|id|String| Inherited from [entity](../resources/entity.md)|
|version|String|Version of the entity.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "id": "String (identifier)",
  "displayName": "String",
  "fileHash": "String",
  "file": "binary",
  "version": "String"
}
```

