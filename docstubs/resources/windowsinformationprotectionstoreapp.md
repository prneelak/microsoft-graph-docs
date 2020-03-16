---
title: "windowsInformationProtectionStoreApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionStoreApp resource type


Namespace: microsoft.graph




Inherits from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|denied|Boolean|If true, app is denied protection or exemption. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|description|String|The app's description. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|displayName|String|App display name. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|productName|String|The product name. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|publisherName|String|The publisher name Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```

