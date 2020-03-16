---
title: "omaSettingBase64 resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# omaSettingBase64 resource type


Namespace: microsoft.graph




Inherits from [omaSetting](../resources/omasetting.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description. Inherited from [omaSetting](../resources/omasetting.md)|
|displayName|String|Display Name. Inherited from [omaSetting](../resources/omasetting.md)|
|fileName|String|File name associated with the Value property (*.cer | *.crt | *.p7b | *.bin).|
|omaUri|String|OMA. Inherited from [omaSetting](../resources/omasetting.md)|
|value|String|Value. (Base64 encoded string)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```

