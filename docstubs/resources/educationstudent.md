---
title: "educationStudent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationStudent resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|birthDate|Date||
|externalId|String||
|gender|Enumeration|. Possible values are: `female`, `male`, `other`, `unknownFutureValue`.|
|grade|String||
|graduationYear|String||
|studentNumber|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "Date",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```

