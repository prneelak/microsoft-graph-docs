---
title: "Update invitation"
description: "Update the properties of a invitation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update invitation

Namespace: microsoft.graph

Update the properties of a [invitation](../resources/invitation.md) object.

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
PATCH /invitations/{invitationsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [invitation](../resources/invitation.md) object.

The following table shows the properties that are required when you create the [invitation](../resources/invitation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|invitedUserDisplayName|String||
|invitedUserType|String||
|invitedUserEmailAddress|String||
|invitedUserMessageInfo|[invitedUserMessageInfo](../resources/invitedusermessageinfo.md)||
|sendInvitationMessage|Boolean||
|inviteRedirectUrl|String||
|inviteRedeemUrl|String||
|status|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [invitation](../resources/invitation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_invitation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}
Content-type: application/json
Content-length: 902

{
  "@odata.type": "#microsoft.graph.invitation",
  "invitedUserDisplayName": "Invited User Display Name value",
  "invitedUserType": "Invited User Type value",
  "invitedUserEmailAddress": "Invited User Email Address value",
  "invitedUserMessageInfo": {
    "@odata.type": "microsoft.graph.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "name": "Name value",
          "address": "Address value"
        }
      }
    ],
    "messageLanguage": "Message Language value",
    "customizedMessageBody": "Customized Message Body value"
  },
  "sendInvitationMessage": true,
  "inviteRedirectUrl": "https://example.com/inviteRedirectUrl/",
  "inviteRedeemUrl": "https://example.com/inviteRedeemUrl/",
  "status": "Status value"
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
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.invitation",
  "id": "66d9b20c-b20c-66d9-0cb2-d9660cb2d966",
  "invitedUserDisplayName": "Invited User Display Name value",
  "invitedUserType": "Invited User Type value",
  "invitedUserEmailAddress": "Invited User Email Address value",
  "invitedUserMessageInfo": {
    "@odata.type": "microsoft.graph.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "name": "Name value",
          "address": "Address value"
        }
      }
    ],
    "messageLanguage": "Message Language value",
    "customizedMessageBody": "Customized Message Body value"
  },
  "sendInvitationMessage": true,
  "inviteRedirectUrl": "https://example.com/inviteRedirectUrl/",
  "inviteRedeemUrl": "https://example.com/inviteRedeemUrl/",
  "status": "Status value"
}
```

