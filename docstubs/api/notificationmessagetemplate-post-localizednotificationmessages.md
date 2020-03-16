---
title: "Add localizedNotificationMessages"
description: "Add localizedNotificationMessages by posting to the localizedNotificationMessages collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add localizedNotificationMessages

Namespace: microsoft.graph

Add localizedNotificationMessages by posting to the localizedNotificationMessages collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.

The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/localizednotificationmessage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|locale|String|The Locale for which this message is destined.|
|subject|String|The Message Template Subject.|
|messageTemplate|String|The Message Template content.|
|isDefault|Boolean|Flag to indicate whether or not this is the default locale for language fallback. This flag can only be set. To unset, set this property to true on another Localized Notification Message.|



## Response
If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/localizednotificationmessage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_localizednotificationmessage_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localizednotificationmessage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "0f4e69e0-69e0-0f4e-e069-4e0fe0694e0f",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

