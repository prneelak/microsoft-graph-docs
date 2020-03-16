---
title: "domain resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# domain resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List domains](../api/domain-list.md)|[domain](../resources/domain.md) collection|List properties and relationships of the [domain](../resources/domain.md) objects.|
|[Get domain](../api/domain-get.md)|[domain](../resources/domain.md)|Read properties and relationships of the [domain](../resources/domain.md) object.|
|[Create domain](../api/domain-post-domains.md)|[domain](../resources/domain.md)|Create a new [domain](../resources/domain.md) object.|
|[Delete domain](../api/domain-delete.md)|None|Deletes a [domain](../resources/domain.md).|
|[Update domain](../api/domain-update.md)|[domain](../resources/domain.md)|Update the properties of a [domain](../resources/domain.md) object.|
|[forceDelete](../api/domain-forcedelete.md)|None||
|[verify](../api/domain-verify.md)|[domain](../resources/domain.md)||
|[List serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md) collection|Get the domainDnsRecords from the serviceConfigurationRecords navigation property.|
|[Add serviceConfigurationRecords](../api/domain-post-serviceconfigurationrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Add serviceConfigurationRecords by posting to the serviceConfigurationRecords collection.|
|[List verificationDnsRecords](../api/domain-list-verificationdnsrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md) collection|Get the domainDnsRecords from the verificationDnsRecords navigation property.|
|[Add verificationDnsRecords](../api/domain-post-verificationdnsrecords.md)|[domainDnsRecord](../resources/domaindnsrecord.md)|Add verificationDnsRecords by posting to the verificationDnsRecords collection.|
|[List domainNameReferences](../api/domain-list-domainnamereferences.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the domainNameReferences navigation property.|
|[Create domainNameReferences](../api/domain-post-domainnamereferences.md)|[directoryObject](../resources/directoryobject.md)|Create domainNameReferences by posting to the domainNameReferences collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationType|String||
|availabilityStatus|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isAdminManaged|Boolean||
|isDefault|Boolean||
|isInitial|Boolean||
|isRoot|Boolean||
|isVerified|Boolean||
|manufacturer|String||
|model|String||
|passwordNotificationWindowInDays|Int32||
|passwordValidityPeriodInDays|Int32||
|state|[domainState](../resources/domainstate.md)||
|supportedServices|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|domainNameReferences|[directoryObject](../resources/directoryobject.md) collection||
|serviceConfigurationRecords|[domainDnsRecord](../resources/domaindnsrecord.md) collection||
|verificationDnsRecords|[domainDnsRecord](../resources/domaindnsrecord.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.domain",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domain",
  "id": "String (identifier)",
  "authenticationType": "String",
  "availabilityStatus": "String",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "manufacturer": "String",
  "model": "String",
  "passwordNotificationWindowInDays": 1024,
  "passwordValidityPeriodInDays": 1024,
  "supportedServices": [
    "String"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState",
    "status": "String",
    "operation": "String",
    "lastActionDateTime": "String (timestamp)"
  }
}
```

