---
title: "domainDnsMxRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domainDnsMxRecord resource type


Namespace: microsoft.graph




Inherits from [domainDnsRecord](../resources/domaindnsrecord.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsMxRecords](../api/domaindnsmxrecord-list.md)|[domainDnsMxRecord](../resources/domaindnsmxrecord.md) collection|List properties and relationships of the [domainDnsMxRecord](../resources/domaindnsmxrecord.md) objects.|
|[Get domainDnsMxRecord](../api/domaindnsmxrecord-get.md)|[domainDnsMxRecord](../resources/domaindnsmxrecord.md)|Read properties and relationships of the [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.|
|[Create domainDnsMxRecord](../api/domaindnsmxrecord-create.md)|[domainDnsMxRecord](../resources/domaindnsmxrecord.md)|Create a new [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.|
|[Delete domainDnsMxRecord](../api/domaindnsmxrecord-delete.md)|None|Deletes a [domainDnsMxRecord](../resources/domaindnsmxrecord.md).|
|[Update domainDnsMxRecord](../api/domaindnsmxrecord-update.md)|[domainDnsMxRecord](../resources/domaindnsmxrecord.md)|Update the properties of a [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|mailExchange|String||
|preference|Int32||
|recordType|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domainDnsMxRecord",
  "baseType": "microsoft.graph.domainDnsRecord",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsMxRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024,
  "mailExchange": "String",
  "preference": 1024
}
```

