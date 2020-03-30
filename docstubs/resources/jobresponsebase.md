---
title: "jobResponseBase resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# jobResponseBase resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get jobResponseBase](../api/jobresponsebase-get.md)|[jobResponseBase](../resources/jobresponsebase.md)|Read properties and relationships of the [jobResponseBase](../resources/jobresponsebase.md) object.|
|[Update jobResponseBase](../api/jobresponsebase-update.md)|[jobResponseBase](../resources/jobresponsebase.md)|Update the properties of a [jobResponseBase](../resources/jobresponsebase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|error|[classificationError](../resources/classificationerror.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|startDateTime|DateTimeOffset||
|status|String||
|tenantId|String||
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.jobResponseBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "id": "String (identifier)",
  "type": "String",
  "status": "String",
  "tenantId": "String",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
  }
}
```

