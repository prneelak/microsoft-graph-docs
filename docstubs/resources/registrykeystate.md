---
title: "registryKeyState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# registryKeyState resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|hive|Enumeration|. Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`, `unknownFutureValue`.|
|key|String||
|oldKey|String||
|oldValueData|String||
|oldValueName|String||
|operation|Enumeration|. Possible values are: `unknown`, `create`, `modify`, `delete`, `unknownFutureValue`.|
|processId|Int32||
|valueData|String||
|valueName|String||
|valueType|Enumeration|. Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registryKeyState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registryKeyState",
  "hive": "String",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "String",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "String"
}
```

