---
title: "sendMail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# sendMail

Namespace: microsoft.graph



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
POST /me/managedDevices/{managedDeviceId}/users/{userId}/sendMail
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|Message|[message](../resources/message.md)||
|SaveToSentItems|Boolean||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/users/{userId}/sendMail

Content-type: application/json
Content-length: 2653

{
  "Message": {
    "@odata.type": "#microsoft.graph.message",
    "id": "c3033aca-3aca-c303-ca3a-03c3ca3a03c3",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "receivedDateTime": "2016-12-31T23:59:18.1123015+03:00",
    "sentDateTime": "2016-12-31T23:58:04.0840241+03:00",
    "hasAttachments": true,
    "internetMessageId": "Internet Message Id value",
    "internetMessageHeaders": [
      {
        "@odata.type": "microsoft.graph.internetMessageHeader"
      }
    ],
    "subject": "Subject value",
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "bodyPreview": "Body Preview value",
    "importance": "String",
    "parentFolderId": "Parent Folder Id value",
    "sender": {
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "address": "Address value"
      }
    },
    "from": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "toRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "bccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "replyTo": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "conversationId": "Conversation Id value",
    "conversationIndex": "Y29udmVyc2F0aW9uSW5kZXg=",
    "uniqueBody": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "isDeliveryReceiptRequested": true,
    "isReadReceiptRequested": true,
    "isRead": true,
    "isDraft": true,
    "webLink": "Web Link value",
    "mentionsPreview": {
      "@odata.type": "microsoft.graph.mentionsPreview",
      "isMentioned": true
    },
    "inferenceClassification": "String",
    "unsubscribeData": [
      "Unsubscribe Data value"
    ],
    "unsubscribeEnabled": true,
    "flag": {
      "@odata.type": "microsoft.graph.followupFlag",
      "completedDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "dueDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "startDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "flagStatus": "String"
    }
  },
  "SaveToSentItems": true
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
HTTP/1.1 204 No Content
```

