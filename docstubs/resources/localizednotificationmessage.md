---
title: "localizedNotificationMessage resource type"
description: "The text content of a Notification Message Template for the specified locale."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# localizedNotificationMessage resource type


Namespace: microsoft.graph

The text content of a Notification Message Template for the specified locale.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get localizedNotificationMessage](../api/localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Read properties and relationships of the [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.|
|[Update localizedNotificationMessage](../api/localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Update the properties of a [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.|
|[List localizedNotificationMessages](../api/notificationmessagetemplate-list-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection|Get the localizedNotificationMessages from the localizedNotificationMessages navigation property.|
|[Add localizedNotificationMessages](../api/notificationmessagetemplate-post-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Add localizedNotificationMessages by posting to the localizedNotificationMessages collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|Flag to indicate whether or not this is the default locale for language fallback. This flag can only be set. To unset, set this property to true on another Localized Notification Message.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|locale|String|The Locale for which this message is destined.|
|messageTemplate|String|The Message Template content.|
|subject|String|The Message Template Subject.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```

