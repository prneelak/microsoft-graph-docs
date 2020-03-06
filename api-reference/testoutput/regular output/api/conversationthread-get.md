---
title: "Get conversationThread"
description: "Read properties and relationships of the conversationThread object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get conversationThread

Namespace: microsoft.graph

Read properties and relationships of the [conversationThread](../resources/conversationthread.md) object.

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
GET /groups/{groupsId}/threads/{conversationThreadId}
GET /me/joinedTeams/{groupId}/threads/{conversationThreadId}
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}
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
If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/threads/{conversationThreadId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 745

{
  "value": {
    "@odata.type": "#microsoft.graph.conversationThread",
    "id": "a03f7a8a-7a8a-a03f-8a7a-3fa08a7a3fa0",
    "toRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "name": "Name value",
          "address": "Address value"
        }
      }
    ],
    "topic": "Topic value",
    "hasAttachments": true,
    "lastDeliveredDateTime": "2017-01-01T00:02:10.6155614+03:00",
    "uniqueSenders": [
      "Unique Senders value"
    ],
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "preview": "Preview value",
    "isLocked": true
  }
}
```

