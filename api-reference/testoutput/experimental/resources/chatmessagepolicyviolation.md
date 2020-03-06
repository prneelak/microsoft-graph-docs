---
title: "chatMessagePolicyViolation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# chatMessagePolicyViolation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|dlpAction|Enumeration|. Possible values are: `none`, `notifySender`, `blockAccess`, `blockAccessExternal`.|
|justificationText|String||
|policyTip|[chatMessagePolicyViolationPolicyTip](../resources/chatmessagepolicyviolationpolicytip.md)||
|userAction|Enumeration|. Possible values are: `none`, `override`, `reportFalsePositive`.|
|verdictDetails|Enumeration|. Possible values are: `none`, `allowFalsePositiveOverride`, `allowOverrideWithoutJustification`, `allowOverrideWithJustification`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessagePolicyViolation",
  "dlpAction": "String",
  "justificationText": "String",
  "policyTip": {
    "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip",
    "generalText": "String",
    "complianceUrl": "String",
    "matchedConditionDescriptions": [
      "String"
    ]
  },
  "userAction": "String",
  "verdictDetails": "String"
}
```

