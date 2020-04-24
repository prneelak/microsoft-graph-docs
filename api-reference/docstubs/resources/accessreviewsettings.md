---
title: "accessReviewSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessReviewSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRecommendationsEnabled|Boolean|**TODO: Add Description**|
|activityDurationInDays|Int32|**TODO: Add Description**|
|autoApplyReviewResultsEnabled|Boolean|**TODO: Add Description**|
|autoReviewEnabled|Boolean|**TODO: Add Description**|
|autoReviewSettings|[autoReviewSettings](../resources/autoreviewsettings.md)|**TODO: Add Description**|
|justificationRequiredOnApproval|Boolean|**TODO: Add Description**|
|mailNotificationsEnabled|Boolean|**TODO: Add Description**|
|recurrenceSettings|[accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md)|**TODO: Add Description**|
|remindersEnabled|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewSettings",
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,
  "justificationRequiredOnApproval": true,
  "recurrenceSettings": {
    "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings",
    "recurrenceType": "String",
    "recurrenceEndType": "String",
    "durationInDays": 1024,
    "recurrenceCount": 1024
  },
  "autoReviewEnabled": true,
  "activityDurationInDays": 1024,
  "autoReviewSettings": {
    "@odata.type": "microsoft.graph.autoReviewSettings",
    "notReviewedResult": "String"
  },
  "autoApplyReviewResultsEnabled": true,
  "accessRecommendationsEnabled": true
}
```

