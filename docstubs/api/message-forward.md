---
title: "forward"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# forward

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
POST /me/messages/{messageId}/forward
POST /users/{usersId}/messages/{messageId}/forward
POST /me/mailFolders/{mailFolderId}/messages/{messageId}/forward
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
|ToRecipients|[recipient](../resources/recipient.md) collection||
|Message|[message](../resources/message.md)||
|Comment|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "message_forward"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/messages/{messageId}/forward

Content-type: application/json
Content-length: 2016

{
  "ToRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "Message": {
    "@odata.type": "#microsoft.graph.message",
    "id": "08dbcd95-cd95-08db-95cd-db0895cddb08",
    "createdDateTime": "2016-12-31T23:56:44.0896282+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:48.4379164+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "receivedDateTime": "2017-01-01T00:03:20.76913+03:00",
    "sentDateTime": "2016-12-31T23:59:43.2025324+03:00",
    "hasAttachments": true,
    "internetMessageId": "Internet Message Id value",
    "internetMessageHeaders": [
      {
        "@odata.type": "microsoft.graph.internetMessageHeader"
      }
    ],
    "subject": "Subject value",
    "body": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "bodyPreview": "Body Preview value",
    "importance": "String",
    "parentFolderId": "Parent Folder Id value",
    "sender": {
      "@odata.type": "microsoft.graph.recipient"
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
    "inferenceClassification": "String",
    "flag": {
      "@odata.type": "microsoft.graph.followupFlag"
    }
  },
  "Comment": "Comment value"
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

