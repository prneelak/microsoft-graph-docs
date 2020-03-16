---
title: "messageRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# messageRule resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get messageRule](../api/messagerule-get.md)|[messageRule](../resources/messagerule.md)|Read properties and relationships of the [messageRule](../resources/messagerule.md) object.|
|[Update messageRule](../api/messagerule-update.md)|[messageRule](../resources/messagerule.md)|Update the properties of a [messageRule](../resources/messagerule.md) object.|
|[List messageRules](../api/mailfolder-list-messagerules.md)|[messageRule](../resources/messagerule.md) collection|Get the messageRules from the messageRules navigation property.|
|[Add messageRules](../api/mailfolder-post-messagerules.md)|[messageRule](../resources/messagerule.md)|Add messageRules by posting to the messageRules collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[messageRuleActions](../resources/messageruleactions.md)||
|conditions|[messageRulePredicates](../resources/messagerulepredicates.md)||
|displayName|String||
|exceptions|[messageRulePredicates](../resources/messagerulepredicates.md)||
|hasError|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean||
|isReadOnly|Boolean||
|sequence|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.messageRule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messageRule",
  "id": "String (identifier)",
  "displayName": "String",
  "sequence": 1024,
  "conditions": {
    "@odata.type": "microsoft.graph.messageRulePredicates"
  },
  "actions": {
    "@odata.type": "microsoft.graph.messageRuleActions"
  },
  "exceptions": {
    "@odata.type": "microsoft.graph.messageRulePredicates"
  },
  "isEnabled": true,
  "hasError": true,
  "isReadOnly": true
}
```

