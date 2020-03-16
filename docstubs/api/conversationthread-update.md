---
title: "Update conversationThread"
description: "Update the properties of a conversationThread object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update conversationThread

Namespace: microsoft.graph

Update the properties of a [conversationThread](../resources/conversationthread.md) object.

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
PATCH /groups/{groupsId}/threads/{conversationThreadId}
PATCH /me/joinedTeams/{groupId}/threads/{conversationThreadId}
PATCH /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [conversationThread](../resources/conversationthread.md) object.

The following table shows the properties that are required when you create the [conversationThread](../resources/conversationthread.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|toRecipients|[recipient](../resources/recipient.md) collection||
|topic|String||
|hasAttachments|Boolean||
|lastDeliveredDateTime|DateTimeOffset||
|uniqueSenders|String collection||
|ccRecipients|[recipient](../resources/recipient.md) collection||
|preview|String||
|isLocked|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [conversationThread](../resources/conversationthread.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/groups/{groupsId}/threads/{conversationThreadId}
Content-type: application/json
Content-length: 627

{
  "@odata.type": "#microsoft.graph.conversationThread",
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
  "lastDeliveredDateTime": "2017-01-01T00:00:23.2016934+03:00",
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
Content-Length: 676

{
  "@odata.type": "#microsoft.graph.conversationThread",
  "id": "30cfca13-ca13-30cf-13ca-cf3013cacf30",
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
  "lastDeliveredDateTime": "2017-01-01T00:00:23.2016934+03:00",
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
```

