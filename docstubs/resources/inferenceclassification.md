---
title: "inferenceClassification resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# inferenceClassification resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get inferenceClassification](../api/inferenceclassification-get.md)|[inferenceClassification](../resources/inferenceclassification.md)|Read properties and relationships of the [inferenceClassification](../resources/inferenceclassification.md) object.|
|[Update inferenceClassification](../api/inferenceclassification-update.md)|[inferenceClassification](../resources/inferenceclassification.md)|Update the properties of a [inferenceClassification](../resources/inferenceclassification.md) object.|
|[List overrides](../api/inferenceclassification-list-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection|Get the inferenceClassificationOverrides from the overrides navigation property.|
|[Add overrides](../api/inferenceclassification-post-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Add overrides by posting to the overrides collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|overrides|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.inferenceClassification",
  "id": "String (identifier)"
}
```

