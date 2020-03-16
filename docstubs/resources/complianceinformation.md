---
title: "complianceInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# complianceInformation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certificationControls|[certificationControl](../resources/certificationcontrol.md) collection||
|certificationName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceInformation",
  "certificationControls": [
    {
      "@odata.type": "microsoft.graph.certificationControl",
      "name": "String",
      "url": "String"
    }
  ],
  "certificationName": "String"
}
```

