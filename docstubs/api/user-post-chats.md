---
title: "Create chats"
description: "Create a new chats object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create chats

Namespace: microsoft.graph

Create a new chats object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/chats
POST /invitations/{invitationsId}/invitedUser/chats
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [chat](../resources/chat.md) object.

The following table shows the properties that are required when you create the [chat](../resources/chat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|topic|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [chat](../resources/chat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_chat_from_chats"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/chats
Content-Type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.chat",
  "topic": "Topic value",
  "lastUpdatedDateTime": "2017-01-01T00:01:54.4720513+03:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.chat",
  "id": "26ce78f1-78f1-26ce-f178-ce26f178ce26",
  "topic": "Topic value",
  "createdDateTime": "2017-01-01T00:00:27.9270493+03:00",
  "lastUpdatedDateTime": "2017-01-01T00:01:54.4720513+03:00"
}
```

