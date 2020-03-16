---
title: "invitation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# invitation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List invitations](../api/invitation-list.md)|[invitation](../resources/invitation.md) collection|List properties and relationships of the [invitation](../resources/invitation.md) objects.|
|[Get invitation](../api/invitation-get.md)|[invitation](../resources/invitation.md)|Read properties and relationships of the [invitation](../resources/invitation.md) object.|
|[Create invitation](../api/invitation-post-invitations.md)|[invitation](../resources/invitation.md)|Create a new [invitation](../resources/invitation.md) object.|
|[Delete invitation](../api/invitation-delete.md)|None|Deletes a [invitation](../resources/invitation.md).|
|[Update invitation](../api/invitation-update.md)|[invitation](../resources/invitation.md)|Update the properties of a [invitation](../resources/invitation.md) object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|invitedUserDisplayName|String||
|invitedUserEmailAddress|String||
|invitedUserMessageInfo|[invitedUserMessageInfo](../resources/invitedusermessageinfo.md)||
|invitedUserType|String||
|inviteRedeemUrl|String||
|inviteRedirectUrl|String||
|sendInvitationMessage|Boolean||
|status|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|invitedUser|[user](../resources/user.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invitation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.invitation",
  "id": "String (identifier)",
  "invitedUserDisplayName": "String",
  "invitedUserType": "String",
  "invitedUserEmailAddress": "String",
  "invitedUserMessageInfo": {
    "@odata.type": "microsoft.graph.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "address": "String"
        }
      }
    ],
    "messageLanguage": "String",
    "customizedMessageBody": "String"
  },
  "sendInvitationMessage": true,
  "inviteRedirectUrl": "String",
  "inviteRedeemUrl": "String",
  "status": "String"
}
```

