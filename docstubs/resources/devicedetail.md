---
title: "deviceDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceDetail resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|browser|String||
|deviceId|String||
|displayName|String||
|isCompliant|Boolean||
|isManaged|Boolean||
|operatingSystem|String||
|trustType|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceDetail",
  "deviceId": "String",
  "displayName": "String",
  "operatingSystem": "String",
  "browser": "String",
  "isCompliant": true,
  "isManaged": true,
  "trustType": "String"
}
```

