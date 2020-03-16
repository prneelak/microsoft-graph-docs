---
title: "teamMemberSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamMemberSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowAddRemoveApps|Boolean||
|allowCreateUpdateChannels|Boolean||
|allowCreateUpdateRemoveConnectors|Boolean||
|allowCreateUpdateRemoveTabs|Boolean||
|allowDeleteChannels|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamMemberSettings",
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

