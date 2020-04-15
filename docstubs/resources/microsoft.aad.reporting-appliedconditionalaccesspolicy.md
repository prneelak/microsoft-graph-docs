---
title: "appliedConditionalAccessPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appliedConditionalAccessPolicy resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|conditionsNotSatisfied|Enumeration| Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|conditionsSatisfied|Enumeration| Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|displayName|String||
|enforcedGrantControls|String collection||
|enforcedSessionControls|String collection||
|id|String||
|result|Enumeration| Possible values are: `success`, `failure`, `notApplied`, `notEnabled`, `unknown`, `unknownFutureValue`, `reportOnlySuccess`, `reportOnlyFailure`, `reportOnlyNotApplied`, `reportOnlyInterrupted`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.appliedConditionalAccessPolicy"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.appliedConditionalAccessPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "enforcedGrantControls": [
    "String"
  ],
  "enforcedSessionControls": [
    "String"
  ],
  "conditionsSatisfied": "String",
  "conditionsNotSatisfied": "String",
  "result": "String"
}
```

