---
title: "Update mention"
description: "Update the properties of a mention object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mention

Namespace: microsoft.graph

Update the properties of a [mention](../resources/mention.md) object.

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
PATCH /me/messages/{messageId}/mentions/{mentionId}
PATCH /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions/{mentionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [mention](../resources/mention.md) object.

The following table shows the properties that are required when you create the [mention](../resources/mention.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|mentioned|[emailAddress](../resources/emailaddress.md)||
|mentionText|String||
|clientReference|String||
|createdBy|[emailAddress](../resources/emailaddress.md)||
|createdDateTime|DateTimeOffset||
|serverCreatedDateTime|DateTimeOffset||
|deepLink|String||
|application|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [mention](../resources/mention.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mention"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/messages/{messageId}/mentions/{mentionId}
Content-type: application/json
Content-length: 485

{
  "@odata.type": "#microsoft.graph.mention",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  },
  "mentionText": "Mention Text value",
  "clientReference": "Client Reference value",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "serverCreatedDateTime": "2016-12-31T23:58:44.2523756+00:00",
  "deepLink": "Deep Link value",
  "application": "Application value"
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
Content-Length: 593

{
  "@odata.type": "#microsoft.graph.mention",
  "id": "6c3645bd-45bd-6c36-bd45-366cbd45366c",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  },
  "mentionText": "Mention Text value",
  "clientReference": "Client Reference value",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
  "serverCreatedDateTime": "2016-12-31T23:58:44.2523756+00:00",
  "deepLink": "Deep Link value",
  "application": "Application value"
}
```

