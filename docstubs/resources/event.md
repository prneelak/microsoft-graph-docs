---
title: "event resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# event resource type


Namespace: microsoft.graph




Inherits from [outlookItem](../resources/outlookitem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read properties and relationships of the [event](../resources/event.md) object.|
|[Update event](../api/event-update.md)|[event](../resources/event.md)|Update the properties of a [event](../resources/event.md) object.|
|[delta](../api/event-delta.md)|[event](../resources/event.md) collection||
|[dismissReminder](../api/event-dismissreminder.md)|None||
|[snoozeReminder](../api/event-snoozereminder.md)|None||
|[accept](../api/event-accept.md)|None||
|[decline](../api/event-decline.md)|None||
|[tentativelyAccept](../api/event-tentativelyaccept.md)|None||
|[List attachments](../api/event-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/event-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|
|[List singleValueExtendedProperties](../api/event-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/event-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/event-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/event-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read properties and relationships of the [calendar](../resources/calendar.md) object.|
|[List instances](../api/event-list-instances.md)|[event](../resources/event.md) collection|Get the events from the instances navigation property.|
|[Add instances](../api/event-post-instances.md)|[event](../resources/event.md)|Add instances by posting to the instances collection.|
|[List extensions](../api/event-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/event-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendees|[attendee](../resources/attendee.md) collection||
|body|[itemBody](../resources/itembody.md)||
|bodyPreview|String||
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|hasAttachments|Boolean||
|iCalUId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration|. Possible values are: `low`, `normal`, `high`.|
|isAllDay|Boolean||
|isCancelled|Boolean||
|isOrganizer|Boolean||
|isReminderOn|Boolean||
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|location|[location](../resources/location.md)||
|locations|[location](../resources/location.md) collection||
|onlineMeetingUrl|String||
|organizer|[recipient](../resources/recipient.md)||
|originalEndTimeZone|String||
|originalStart|DateTimeOffset||
|originalStartTimeZone|String||
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)||
|reminderMinutesBeforeStart|Int32||
|responseRequested|Boolean||
|responseStatus|[responseStatus](../resources/responsestatus.md)||
|sensitivity|Enumeration|. Possible values are: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String||
|showAs|Enumeration|. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|subject|String||
|type|Enumeration|. Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|webLink|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection||
|calendar|[calendar](../resources/calendar.md)||
|extensions|[extension](../resources/extension.md) collection||
|instances|[event](../resources/event.md) collection||
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.event",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.event",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ],
  "originalStartTimeZone": "String",
  "originalEndTimeZone": "String",
  "responseStatus": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "String (timestamp)"
  },
  "iCalUId": "String",
  "reminderMinutesBeforeStart": 1024,
  "isReminderOn": true,
  "hasAttachments": true,
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "String"
  },
  "bodyPreview": "String",
  "importance": "String",
  "sensitivity": "String",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "String",
    "timeZone": "String"
  },
  "originalStart": "String (timestamp)",
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "location": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "String",
    "locationEmailAddress": "String",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "street": "String",
      "city": "String",
      "state": "String",
      "countryOrRegion": "String",
      "postalCode": "String"
    },
    "locationUri": "String",
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitude": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationType": "String",
    "uniqueId": "String",
    "uniqueIdType": "String"
  },
  "locations": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 1024,
      "month": 1024,
      "dayOfMonth": 1024,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "String",
      "numberOfOccurrences": 1024
    }
  },
  "responseRequested": true,
  "seriesMasterId": "String",
  "showAs": "String",
  "type": "String",
  "attendees": [
    {
      "@odata.type": "microsoft.graph.attendee",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "String",
        "address": "String"
      },
      "type": "String",
      "status": {
        "@odata.type": "microsoft.graph.responseStatus"
      }
    }
  ],
  "organizer": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "webLink": "String",
  "onlineMeetingUrl": "String"
}
```

