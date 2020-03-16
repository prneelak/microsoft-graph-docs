---
title: "Create invitation"
description: "Create a new invitation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create invitation

Namespace: microsoft.graph

Create a new [invitation](../resources/invitation.md) object.

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
POST /invitations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [invitation](../resources/invitation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_invitation_from_invitations"
}
-->
``` http
POST https://graph.microsoft.com/localtest/invitations
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
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.invitation",
  "id": "a8c61b17-1b17-a8c6-171b-c6a8171bc6a8",
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

