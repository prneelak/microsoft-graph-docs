---
title: "activityHistoryItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# activityHistoryItem resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get activityHistoryItem](../api/activityhistoryitem-get.md)|[activityHistoryItem](../resources/activityhistoryitem.md)|Read properties and relationships of the [activityHistoryItem](../resources/activityhistoryitem.md) object.|
|[Update activityHistoryItem](../api/activityhistoryitem-update.md)|[activityHistoryItem](../resources/activityhistoryitem.md)|Update the properties of a [activityHistoryItem](../resources/activityhistoryitem.md) object.|
|[Get userActivity](../api/useractivity-get.md)|[userActivity](../resources/useractivity.md)|Read properties and relationships of the [userActivity](../resources/useractivity.md) object.|
|[List historyItems](../api/useractivity-list-historyitems.md)|[activityHistoryItem](../resources/activityhistoryitem.md) collection|Get the activityHistoryItems from the historyItems navigation property.|
|[Add historyItems](../api/useractivity-post-historyitems.md)|[activityHistoryItem](../resources/activityhistoryitem.md)|Add historyItems by posting to the historyItems collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeDurationSeconds|Int32||
|createdDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActiveDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|startedDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|userTimezone|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activity|[userActivity](../resources/useractivity.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "id": "String (identifier)",
  "status": "String",
  "activeDurationSeconds": 1024,
  "createdDateTime": "String (timestamp)",
  "lastActiveDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "startedDateTime": "String (timestamp)",
  "userTimezone": "String"
}
```

