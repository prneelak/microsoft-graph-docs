---
title: "targetResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# targetResource resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|groupType|Enumeration|. Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|
|id|String||
|modifiedProperties|[modifiedProperty](../resources/modifiedproperty.md) collection||
|type|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.targetResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.modifiedProperty",
      "oldValue": "String",
      "newValue": "String"
    }
  ]
}
```

