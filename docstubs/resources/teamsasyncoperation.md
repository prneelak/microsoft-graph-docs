---
title: "teamsAsyncOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsAsyncOperation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsAsyncOperation](../api/teamsasyncoperation-get.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Read properties and relationships of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|
|[Update teamsAsyncOperation](../api/teamsasyncoperation-update.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Update the properties of a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|
|[List operations](../api/team-list-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|Get the teamsAsyncOperations from the operations navigation property.|
|[Add operations](../api/team-post-operations.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attemptsCount|Int32||
|createdDateTime|DateTimeOffset||
|error|[operationError](../resources/operationerror.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActionDateTime|DateTimeOffset||
|operationType|Enumeration|. Possible values are: `invalid`, `cloneTeam`, `archiveTeam`, `unarchiveTeam`, `createTeam`, `unknownFutureValue`.|
|status|Enumeration|. Possible values are: `invalid`, `notStarted`, `inProgress`, `succeeded`, `failed`, `unknownFutureValue`.|
|targetResourceId|String||
|targetResourceLocation|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "id": "String (identifier)",
  "operationType": "String",
  "createdDateTime": "String (timestamp)",
  "status": "String",
  "lastActionDateTime": "String (timestamp)",
  "attemptsCount": 1024,
  "targetResourceId": "String",
  "targetResourceLocation": "String",
  "error": {
    "@odata.type": "microsoft.graph.operationError"
  }
}
```

