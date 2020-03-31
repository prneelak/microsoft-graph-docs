---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

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
GET /me/messages/delta
GET /users/{usersId}/messages/delta
GET /me/mailFolders/{mailFolderId}/messages/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [message](../resources/message.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "message_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.message)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2239

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "id": "2924937d-937d-2924-7d93-24297d932429",
      "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
      "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "receivedDateTime": "2017-01-01T00:03:20.0381972+03:00",
      "sentDateTime": "2016-12-31T23:58:23.5347717+03:00",
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
      "mentionsPreview": {
        "@odata.type": "microsoft.graph.mentionsPreview"
      },
      "inferenceClassification": "String",
      "unsubscribeData": [
        "Unsubscribe Data value"
      ],
      "unsubscribeEnabled": true,
      "flag": {
        "@odata.type": "microsoft.graph.followupFlag"
      }
    }
  ]
}
```

