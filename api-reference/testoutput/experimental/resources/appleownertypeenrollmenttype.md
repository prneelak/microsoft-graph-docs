---
title: "appleOwnerTypeEnrollmentType resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appleOwnerTypeEnrollmentType resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|enrollmentType|Enumeration|The enrollment type. Possible values are: `unknown`, `device`, `user`.|
|ownerType|Enumeration|The owner type. Possible values are: `unknown`, `company`, `personal`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleOwnerTypeEnrollmentType",
  "ownerType": "String",
  "enrollmentType": "String"
}
```

