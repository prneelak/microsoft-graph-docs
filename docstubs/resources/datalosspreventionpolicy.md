---
title: "dataLossPreventionPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dataLossPreventionPolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get dataLossPreventionPolicy](../api/datalosspreventionpolicy-get.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md)|Read properties and relationships of the [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) object.|
|[Update dataLossPreventionPolicy](../api/datalosspreventionpolicy-update.md)|[dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md)|Update the properties of a [dataLossPreventionPolicy](../resources/datalosspreventionpolicy.md) object.|
|[evaluate](../api/datalosspreventionpolicy-evaluate.md)|[dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataLossPreventionPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataLossPreventionPolicy",
  "id": "String (identifier)",
  "name": "String"
}
```

