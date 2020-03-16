---
title: "remoteLockActionResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# remoteLockActionResult resource type


Namespace: microsoft.graph




Inherits from [deviceActionResult](../resources/deviceactionresult.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionName|String|Action name Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|actionState|Enumeration|State of the action Inherited from [deviceActionResult](../resources/deviceactionresult.md). Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|lastUpdatedDateTime|DateTimeOffset|Time the action state was last updated Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|startDateTime|DateTimeOffset|Time the action was initiated Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|unlockPin|String|Pin to unlock the client|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```

