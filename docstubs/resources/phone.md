---
title: "phone resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# phone resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|language|String||
|number|String||
|region|String||
|type|Enumeration|. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.phone"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.phone",
  "type": "String",
  "number": "String",
  "region": "String",
  "language": "String"
}
```

