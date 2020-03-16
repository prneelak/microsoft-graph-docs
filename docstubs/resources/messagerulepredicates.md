---
title: "messageRulePredicates resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# messageRulePredicates resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|bodyContains|String collection||
|bodyOrSubjectContains|String collection||
|categories|String collection||
|fromAddresses|[recipient](../resources/recipient.md) collection||
|hasAttachments|Boolean||
|headerContains|String collection||
|importance|Enumeration|. Possible values are: `low`, `normal`, `high`.|
|isApprovalRequest|Boolean||
|isAutomaticForward|Boolean||
|isAutomaticReply|Boolean||
|isEncrypted|Boolean||
|isMeetingRequest|Boolean||
|isMeetingResponse|Boolean||
|isNonDeliveryReport|Boolean||
|isPermissionControlled|Boolean||
|isReadReceipt|Boolean||
|isSigned|Boolean||
|isVoicemail|Boolean||
|messageActionFlag|Enumeration|. Possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.|
|notSentToMe|Boolean||
|recipientContains|String collection||
|senderContains|String collection||
|sensitivity|Enumeration|. Possible values are: `normal`, `personal`, `private`, `confidential`.|
|sentCcMe|Boolean||
|sentOnlyToMe|Boolean||
|sentToAddresses|[recipient](../resources/recipient.md) collection||
|sentToMe|Boolean||
|sentToOrCcMe|Boolean||
|subjectContains|String collection||
|withinSizeRange|[sizeRange](../resources/sizerange.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.messageRulePredicates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messageRulePredicates",
  "categories": [
    "String"
  ],
  "subjectContains": [
    "String"
  ],
  "bodyContains": [
    "String"
  ],
  "bodyOrSubjectContains": [
    "String"
  ],
  "senderContains": [
    "String"
  ],
  "recipientContains": [
    "String"
  ],
  "headerContains": [
    "String"
  ],
  "messageActionFlag": "String",
  "importance": "String",
  "sensitivity": "String",
  "fromAddresses": [
    {
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "String",
        "address": "String"
      }
    }
  ],
  "sentToAddresses": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "sentToMe": true,
  "sentOnlyToMe": true,
  "sentCcMe": true,
  "sentToOrCcMe": true,
  "notSentToMe": true,
  "hasAttachments": true,
  "isApprovalRequest": true,
  "isAutomaticForward": true,
  "isAutomaticReply": true,
  "isEncrypted": true,
  "isMeetingRequest": true,
  "isMeetingResponse": true,
  "isNonDeliveryReport": true,
  "isPermissionControlled": true,
  "isReadReceipt": true,
  "isSigned": true,
  "isVoicemail": true,
  "withinSizeRange": {
    "@odata.type": "microsoft.graph.sizeRange",
    "minimumSize": 1024,
    "maximumSize": 1024
  }
}
```

