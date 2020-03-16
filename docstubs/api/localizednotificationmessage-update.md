---
title: "Update localizedNotificationMessage"
description: "Update the properties of a localizedNotificationMessage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update localizedNotificationMessage

Namespace: microsoft.graph

Update the properties of a [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.

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
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/localizednotificationmessage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_localizednotificationmessage"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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

