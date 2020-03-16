---
title: "appConfigurationSettingItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appConfigurationSettingItem resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appConfigKey|String|app configuration key.|
|appConfigKeyType|Enumeration|app configuration key type. Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.|
|appConfigKeyValue|String|app configuration key value.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```

