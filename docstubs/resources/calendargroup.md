---
title: "calendarGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# calendarGroup resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get calendarGroup](../api/calendargroup-get.md)|[calendarGroup](../resources/calendargroup.md)|Read properties and relationships of the [calendarGroup](../resources/calendargroup.md) object.|
|[Update calendarGroup](../api/calendargroup-update.md)|[calendarGroup](../resources/calendargroup.md)|Update the properties of a [calendarGroup](../resources/calendargroup.md) object.|
|[List calendars](../api/calendargroup-list-calendars.md)|[calendar](../resources/calendar.md) collection|Get the calendars from the calendars navigation property.|
|[Add calendars](../api/calendargroup-post-calendars.md)|[calendar](../resources/calendar.md)|Add calendars by posting to the calendars collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String||
|classId|Guid||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|calendars|[calendar](../resources/calendar.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.calendarGroup",
  "id": "String (identifier)",
  "name": "String",
  "classId": "Guid",
  "changeKey": "String"
}
```

