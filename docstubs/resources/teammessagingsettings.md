---
title: "teamMessagingSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamMessagingSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowChannelMentions|Boolean||
|allowOwnerDeleteMessages|Boolean||
|allowTeamMentions|Boolean||
|allowUserDeleteMessages|Boolean||
|allowUserEditMessages|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamMessagingSettings",
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true
}
```

