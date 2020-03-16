---
title: "windowsDeviceADAccount resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsDeviceADAccount resource type


Namespace: microsoft.graph




Inherits from [windowsDeviceAccount](../resources/windowsdeviceaccount.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|domainName|String||
|password|String| Inherited from [windowsDeviceAccount](../resources/windowsdeviceaccount.md)|
|userName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "password": "String",
  "domainName": "String",
  "userName": "String"
}
```

