---
title: "omaSettingInteger resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# omaSettingInteger resource type


Namespace: microsoft.graph




Inherits from [omaSetting](../resources/omasetting.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description. Inherited from [omaSetting](../resources/omasetting.md)|
|displayName|String|Display Name. Inherited from [omaSetting](../resources/omasetting.md)|
|omaUri|String|OMA. Inherited from [omaSetting](../resources/omasetting.md)|
|value|Int32|Value.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```

