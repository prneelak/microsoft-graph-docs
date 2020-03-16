---
title: "mailTips resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mailTips resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|automaticReplies|[automaticRepliesMailTips](../resources/automaticrepliesmailtips.md)||
|customMailTip|String||
|deliveryRestricted|Boolean||
|emailAddress|[emailAddress](../resources/emailaddress.md)||
|error|[mailTipsError](../resources/mailtipserror.md)||
|externalMemberCount|Int32||
|isModerated|Boolean||
|mailboxFull|Boolean||
|maxMessageSize|Int32||
|recipientScope|Enumeration|. Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonPartner`.|
|recipientSuggestions|[recipient](../resources/recipient.md) collection||
|totalMemberCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailTips"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailTips",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "String",
    "address": "String"
  },
  "automaticReplies": {
    "@odata.type": "microsoft.graph.automaticRepliesMailTips",
    "message": "String",
    "messageLanguage": {
      "@odata.type": "microsoft.graph.localeInfo",
      "locale": "String",
      "displayName": "String"
    },
    "scheduledStartTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "scheduledEndTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    }
  },
  "mailboxFull": true,
  "customMailTip": "String",
  "externalMemberCount": 1024,
  "totalMemberCount": 1024,
  "deliveryRestricted": true,
  "isModerated": true,
  "recipientScope": "String",
  "recipientSuggestions": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "maxMessageSize": 1024,
  "error": {
    "@odata.type": "microsoft.graph.mailTipsError",
    "code": "String"
  }
}
```

