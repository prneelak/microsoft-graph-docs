---
title: "alertHistoryState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# alertHistoryState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String||
|assignedTo|String||
|comments|String collection||
|feedback|Enumeration|. Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`, `unknownFutureValue`.|
|status|Enumeration|. Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`, `unknownFutureValue`.|
|updatedDateTime|DateTimeOffset||
|user|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alertHistoryState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.alertHistoryState",
  "appId": "String",
  "assignedTo": "String",
  "comments": [
    "String"
  ],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

