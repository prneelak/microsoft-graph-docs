---
title: "relatedContact resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# relatedContact resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessConsent|Boolean|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|emailAddress|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|relationship|contactRelationship|**TODO: Add Description**. Possible values are: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "id": "String (identifier)",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": true
}
```

