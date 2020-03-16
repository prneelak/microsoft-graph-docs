---
title: "omaSettingStringXml resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# omaSettingStringXml resource type


Namespace: microsoft.graph




Inherits from [omaSetting](../resources/omasetting.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description. Inherited from [omaSetting](../resources/omasetting.md)|
|displayName|String|Display Name. Inherited from [omaSetting](../resources/omasetting.md)|
|fileName|String|File name associated with the Value property (*.xml).|
|omaUri|String|OMA. Inherited from [omaSetting](../resources/omasetting.md)|
|value|Binary|Value. (UTF8 encoded byte array)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```

