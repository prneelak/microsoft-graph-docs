---
title: "calendar resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# calendar resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read properties and relationships of the [calendar](../resources/calendar.md) object.|
|[Update calendar](../api/calendar-update.md)|[calendar](../resources/calendar.md)|Update the properties of a [calendar](../resources/calendar.md) object.|
|[getSchedule](../api/calendar-getschedule.md)|[scheduleInformation](../resources/scheduleinformation.md) collection||
|[List singleValueExtendedProperties](../api/calendar-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/calendar-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/calendar-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/calendar-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List events](../api/calendar-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Add events](../api/calendar-post-events.md)|[event](../resources/event.md)|Add events by posting to the events collection.|
|[List calendarView](../api/calendar-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Add calendarView](../api/calendar-post-calendarview.md)|[event](../resources/event.md)|Add calendarView by posting to the calendarView collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|canEdit|Boolean||
|canShare|Boolean||
|canViewPrivateItems|Boolean||
|changeKey|String||
|color|Enumeration|. Possible values are: `lightBlue`, `lightGreen`, `lightOrange`, `lightGray`, `lightYellow`, `lightTeal`, `lightPink`, `lightBrown`, `lightRed`, `maxColor`, `auto`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|owner|[emailAddress](../resources/emailaddress.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|calendarView|[event](../resources/event.md) collection||
|events|[event](../resources/event.md) collection||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.calendar",
  "id": "String (identifier)",
  "name": "String",
  "color": "String",
  "changeKey": "String",
  "canShare": true,
  "canViewPrivateItems": true,
  "canEdit": true,
  "owner": {
    "@odata.type": "microsoft.graph.emailAddress"
  }
}
```

