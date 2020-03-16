---
title: "List messages"
description: "Get the messages from the messages navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List messages

Namespace: microsoft.graph

Get the messages from the messages navigation property.

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
GET /me/messages
GET /users/{usersId}/messages
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [message](../resources/message.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_message"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/messages
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
Content-Length: 2732

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "id": "f5e9be76-be76-f5e9-76be-e9f576bee9f5",
      "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
      "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "receivedDateTime": "2016-12-31T23:59:09.8646673+03:00",
      "sentDateTime": "2016-12-31T23:57:26.8046857+03:00",
      "hasAttachments": true,
      "internetMessageId": "Internet Message Id value",
      "internetMessageHeaders": [
        {
          "@odata.type": "microsoft.graph.internetMessageHeader",
          "name": "Name value",
          "value": "Value value"
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
      "inferenceClassification": "String",
      "flag": {
        "@odata.type": "microsoft.graph.followupFlag",
        "completedDateTime": {
          "@odata.type": "microsoft.graph.dateTimeTimeZone",
          "dateTime": "Date Time value",
          "timeZone": "Time Zone value"
        },
        "dueDateTime": {
          "@odata.type": "microsoft.graph.dateTimeTimeZone"
        },
        "startDateTime": {
          "@odata.type": "microsoft.graph.dateTimeTimeZone"
        },
        "flagStatus": "String"
      }
    }
  ]
}
```

