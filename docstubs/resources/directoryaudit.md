---
title: "directoryAudit resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# directoryAudit resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get directoryAudit](../api/directoryaudit-get.md)|[directoryAudit](../resources/directoryaudit.md)|Read properties and relationships of the [directoryAudit](../resources/directoryaudit.md) object.|
|[Update directoryAudit](../api/directoryaudit-update.md)|[directoryAudit](../resources/directoryaudit.md)|Update the properties of a [directoryAudit](../resources/directoryaudit.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activityDateTime|DateTimeOffset||
|activityDisplayName|String||
|additionalDetails|[keyValue](../resources/keyvalue.md) collection||
|category|String||
|correlationId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|initiatedBy|[auditActivityInitiator](../resources/auditactivityinitiator.md)||
|loggedByService|String||
|operationType|String||
|result|Enumeration|. Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.|
|resultReason|String||
|targetResources|[targetResource](../resources/targetresource.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryAudit",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryAudit",
  "id": "String (identifier)",
  "category": "String",
  "correlationId": "String",
  "result": "String",
  "resultReason": "String",
  "activityDisplayName": "String",
  "activityDateTime": "String (timestamp)",
  "loggedByService": "String",
  "operationType": "String",
  "initiatedBy": {
    "@odata.type": "microsoft.graph.auditActivityInitiator"
  },
  "targetResources": [
    {
      "@odata.type": "microsoft.graph.targetResource"
    }
  ],
  "additionalDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```

