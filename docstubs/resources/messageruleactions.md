---
title: "messageRuleActions resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# messageRuleActions resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignCategories|String collection||
|copyToFolder|String||
|delete|Boolean||
|forwardAsAttachmentTo|[recipient](../resources/recipient.md) collection||
|forwardTo|[recipient](../resources/recipient.md) collection||
|markAsRead|Boolean||
|markImportance|Enumeration|. Possible values are: `low`, `normal`, `high`.|
|moveToFolder|String||
|permanentDelete|Boolean||
|redirectTo|[recipient](../resources/recipient.md) collection||
|stopProcessingRules|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.messageRuleActions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messageRuleActions",
  "moveToFolder": "String",
  "copyToFolder": "String",
  "delete": true,
  "permanentDelete": true,
  "markAsRead": true,
  "markImportance": "String",
  "forwardTo": [
    {
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "String",
        "address": "String"
      }
    }
  ],
  "forwardAsAttachmentTo": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "redirectTo": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "assignCategories": [
    "String"
  ],
  "stopProcessingRules": true
}
```

