---
title: "domainDnsRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domainDnsRecord resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domainDnsRecords](../api/domaindnsrecord-list.md)|[domainDnsRecord](../resources/domaindnsrecord.md) collection|List properties and relationships of the [domainDnsRecord](../resources/domaindnsrecord.md) objects.|
|[Get domainDnsRecord](../api/domaindnsrecord-get.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Read properties and relationships of the [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Create domainDnsRecord](../api/domaindnsrecord-post-domaindnsrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Create a new [domainDnsRecord](../resources/domaindnsrecord.md) object.|
|[Delete domainDnsRecord](../api/domaindnsrecord-delete.md)|None|Deletes a [domainDnsRecord](../resources/domaindnsrecord.md).|
|[Update domainDnsRecord](../api/domaindnsrecord-update.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Update the properties of a [domainDnsRecord](../resources/domaindnsrecord.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean||
|label|String||
|recordType|String||
|supportedService|String||
|ttl|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}
```

